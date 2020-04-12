云监工
==========

## 架构

| | | | | | | | | |
|-|-|-|-|-|-|-|-|-|
| | | | `/->`<br>UDP | `capturing`<br>延时抓图 | `-->`<br>HEIF | `[disk]`<br>&nbsp; | | |
| `[cam]`<br>&nbsp; | `-->`<br>RTSP | `proxy`<br>分发 | `-->`<br>UDP | `encoding`<br>包装/转码  | `-->`<br>UDP | `streaming`<br>推流 | `-->`<br>RTMP | `[bilibili]`<br>&nbsp; |
| | | | | | | | `\->`<br>RTMP | `[huya]`<br>&nbsp; |
