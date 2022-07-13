# hexo-enhancer-pengber

This is an feature enhancement plugin for `Hexo` based on hexo-enhancer.

I fork the hexo-enhancer on 2022/07/13 and then the author commits on Oct 13, 2021 last time.

hexo-enhancer: https://github.com/sisyphsu/hexo-enhancer#readme
hexo-enhancer中文文档：https://sulin.me/2019/Z726F8.html

##  Introduction

Hexo-enhancer support multiple helpful features as blow:

- Auto generate `title` by filename.
- Auto generate `abbrlink` by filename, with `base32` and `crc32` arithmetic.
- Auto generate `date` by filename, like `Jekyll`.
- Auto generate `categories` by filepath.
- Auto generate `tags` by global pre-configured `tags` and `keywords` in the `_config.yml`.


## My change

### File name

I change the title parsing pattern from 
```
/^.?(\d{4})[-_]?(\d{2})[-_]?(\d{2}).?[-_.@# ]*(.*)$/
```
to
```
/^(.*)[-_.@# ]*.?(\d{4})[-_]?(\d{2})[-_]?(\d{2}).?$/
```
which means the file name should be named like "文章标题_20220713" etc.

## License

MIT
