# MicroProfile Language Server Demo

Demo for MicroProfile Language Server using VS Code

### Setup
Build the following projects and install the extension in VS Code.
- https://github.com/MicroShed/microprofile-language-server
- https://github.com/MicroShed/microprofile-lsp-client-vscode

### Language support for MicroProfile OpenAPI
1. Clone OpenAPI guide
```
git clone https://github.com/OpenLiberty/guide-microprofile-openapi.git
```
2. In VS Code, File -> Open and open the `guide-microprofile-openapi/finish` folder.

#### OpenAPI Annotation Source Actions:
1. Navigate to `src/main/java/io/openliberty/guides/inventory/InventoryResource.java`
1. Delete the entire `@Operation` annotation above `getPropertiesForHost`.
1. Right-click anywhere in the class, choose `Source Action...`, `Generate OpenAPI Annotations`
1. An `@Operation` annotation is generated with fields that you can fill in.

#### OpenAPI Annotation Code Complete:
1. Delete the `@Operation` annotation.  Press Control Space and start typing `@`.  Select the `Operation` code complete, which inserts a code snippet with fields that you can fill in.
1. Delete the `@Parameter` annotation.  Press Control Space and start typing `@`.  Select the `Parameter` code complete, which inserts a code snippet with fields that you can fill in.
