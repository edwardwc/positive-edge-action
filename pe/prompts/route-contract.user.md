Write the edge contract for this route.

Framework: {{framework}}
Route id: {{id}}
Route kind: {{kind}}
Path pattern: {{path}}   (`:name` = one segment, `*name` = one or more segments, `*name?` = zero or more)
Candidate methods: {{methods}}
Route file: {{routeFile}}

## Route source
{{routeSource}}

## Imported modules (resolved from the route file)
{{importedSources}}

## Middleware / shared code that runs for this route
{{middlewareSource}}

## Client-side call sites that reference this path
{{callSites}}

## Framework config
{{frameworkConfig}}
