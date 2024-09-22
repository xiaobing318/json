# Documentation

## Generate documentation

Note on documentation: The source files contain links to the online documentation at https://json.nlohmann.me. This URL
contains the most recent documentation and should also be applicable to previous versions; documentation for deprecated
functions is not removed, but marked deprecated.（文档说明：源文件包含在线文档的链接，网址为 https://json.nlohmann.me。此 URL
包含最新文档，也适用于以前的版本；已弃用的函数的文档不会被删除，但会被标记为已弃用。）

If you want to see the documentation for a specific tag or commit hash, you can generate it as follows (here for tag
`v3.10.2`)（如果您想查看特定标签或提交哈希的文档，您可以按如下方式生成它（此处针对标签`v3.10.2`））:

```shell
git clone https://github.com/nlohmann/json.git
cd json
git checkout v3.10.2
make install_venv serve -C docs/mkdocs
```

Open URL <http://127.0.0.1:8000/> in your browser. Replace from any URL from the source code `https://json.nlohmann.me`
with `http://127.0.0.1:8000` to see the documentation for your tag or commit hash.
