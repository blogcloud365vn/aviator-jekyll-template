---
title: /server
position: 4.6
type: get
description: Hiển thị thông tin các volume mà máy chủ ảo sử dụng
left_code_blocks:
  - code_block: |-
      r = requests.get("http://portalurl/api/v1/server/{instance_id}/list_volume_attached/", token="YOUR_TOKEN_KEY")
      print r.text
    title: Python
    language: python
right_code_blocks:
  - code_block: |-
        [
            {
                "bootable": "true",
                "name": "string",
                "size": 0,
                "volume_id": "string"
            },
        ]

    title: Response
    language: json
---