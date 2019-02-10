# The dokreplayx Format

Binary file format for storing replay data as one file.

| Field Name    | Length          | Description
| ------------- | --------------- | -----------
| Layout Length |              4B | The length of the layout field in bytes
| Patch Length  |              4B | The length of the patch field in bytes
| Reserved      |              8B | Reserved
| Layout        | [Layout Length] | The UTF8 encoded layout data
| Patch         | [Patch Length]  | The UTF8 encoded patch data
