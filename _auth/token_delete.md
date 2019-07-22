---
title: /auth
position: 3.3
type: del
description: Xóa token hiện tại
content_markdown: |-
  API sử dụng để xóa token đang sử dụng
left_code_blocks:
  - code_block: |-
      r = requests.delete("http://portalurl/api/v1/auth/tokens", token="YOUR_TOKEN_KEY")
      print r.text
    title: Python
    language: python
---