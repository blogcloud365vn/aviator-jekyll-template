---
title: Token Delete
position: 1.3
type: delete
description: Xóa token hiện tại
content_markdown: |-
  API sử dụng để xóa token đang sử dụng
  /api/v1/auth/tokens
left_code_blocks:
  - code_block: |-
      r = requests.delete("http://portalurl/api/v1/auth/tokens", token="YOUR_TOKEN_KEY")
      print r.text
    title: Python
    language: python
---