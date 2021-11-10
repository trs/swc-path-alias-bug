`swc` path alias removes parts of file names if they contain periods.

For example, the file `item.service.ts` when imported using a path alias will remove the `.service` from the import.

Adding the full extension (eg: `import ... from "~/item.service.ts"`) seems to resolve this, but editors such as VSCode will complain and suggest to remove the `.ts`.

Importing without the path alias works correctly.
