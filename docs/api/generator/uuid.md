The UUID generator provides random UUIDs that you can feed into your applications. A UUID (Universally Unique Identifier) is a 128-bit label used for information in computer systems. This generator produces version 4 (random) UUIDs.

## Output Keys and Values

| Key  | Description        |
| ---- | ------------------ |
| uuid | the generated UUID |

## Parameters

The UUID generator does not require any additional parameters.

## Example Manifest

```yaml
{% include 'generator-uuid.yaml' %}
```

Example `ExternalSecret` that references the UUID generator:

```yaml
{% include 'generator-uuid-example.yaml' %}
```

Which will generate a `Kind=Secret` with a key called `uuid` that may look like:

```
ea111697-e7d0-452c-a24c-8e396947e865
```
