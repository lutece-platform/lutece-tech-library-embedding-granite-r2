# lutece-tech-library-embedding-granite-r2

Granite Embedding 97M Multilingual R2 ONNX model and tokenizer, packaged for [library-embedding](https://github.com/lutece-platform/lutece-tech-library-embedding).

## Content

`fr/paris/lutece/plugins/embedding/models/granite-r2/` on the classpath:

| File | Content |
|---|---|
| `model.onnx` | `onnx/model_quint8_avx2.onnx` of the model, int8 weights, AVX2 CPU |
| `tokenizer.json` | tokenizer of the model |
| `model.properties` | identifier, 384 dimensions, CLS pooling, no prefix, 512 tokens |
| `NOTICE.txt` | source, revision, license and checksums |

The files are the ones of revision `835ad14087e140460703cf0fae09f97d469d65c2` of
[ibm-granite/granite-embedding-97m-multilingual-r2](https://huggingface.co/ibm-granite/granite-embedding-97m-multilingual-r2), unchanged.

## Usage

Add the artifact next to `library-embedding`; the model is found by its name, `granite-r2`.

```xml
<dependency>
    <groupId>fr.paris.lutece.plugins</groupId>
    <artifactId>library-embedding-granite-r2</artifactId>
    <version>1.0.0-SNAPSHOT</version>
</dependency>
```

## License

The model is published by IBM under the Apache License 2.0.
