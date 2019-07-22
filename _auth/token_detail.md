---
title: /api/v1/auth/tokens
position: 3.2
type: get
description: Hiển thị thông tin chi tiết của token
content_markdown: |-
  API sử dụng để  hiển thị các thông tin đến token
left_code_blocks:
  - code_block: |-
      r = requests.get("http://portalurl/api/v1/auth/tokens", token="YOUR_TOKEN_KEY")
      print r.text
    title: Python
    language: python
right_code_blocks:
  - code_block: |-
      {
        "project_id": string,
        "token_created": "YYYY-MM-DDTh:i:s+07:00",
        "token_expired": "YYYY-MM-DDTh:i:s+07:00",
        "token_key": "user@example.com"
      }
    title: Response
    language: json
---