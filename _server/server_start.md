---
title: /server
position: 4.8
type: post
description: Bật máy chủ ảo
left_code_blocks:
  - code_block: |-
      r = requests.get("http://portalurl/api/v1/server/{instance_id}/start/", token="YOUR_TOKEN_KEY")
      print r.text
    title: Python
    language: python
right_code_blocks:
  - code_block: |-
      {
        "message": "string"
      }

    title: Response
    language: json
---