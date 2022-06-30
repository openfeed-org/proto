# Barchart Openfeed Protobufs

* https://docs.barchart.com/openfeed/#/proto

### Generating Markdown Docs

```bash
docker run --rm \
  -v $(pwd)/.docs:/out \
  -v $(pwd):/protos \
  pseudomuto/protoc-gen-doc --doc_opt=./protos/.docs/markdown.tmpl,proto_markdown.md
```