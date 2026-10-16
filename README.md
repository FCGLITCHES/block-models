# Block image models

Optional on-device image models for the Block Android app. Block ships with Marqo built in and downloads these only when a user picks one,
checking each file's SHA-256 before use. Files are attached to the [v1 release](../../releases/tag/v1).

These are format conversions (ONNX / TFLite) of openly licensed upstream models; no weights were retrained. Each keeps its upstream licence,
included in `licenses/`.

| File | Model | Bytes | Licence | Upstream | SHA-256 |
|---|---|---|---|---|---|
| `opennsfw2.tflite` | OpenNSFW2 / Yahoo | 23,615,868 | MIT implementation; BSD-2-Clause Yahoo model | https://github.com/bhky/opennsfw2 | `2eb4b11e1ccce9af30a1572e39064c6f3c2b799affe112d9b830c223c688cd0a` |
| `nudenet.onnx` | NudeNet 320 | 12,150,158 | AGPL-3.0; Ultralytics-derived weights | https://github.com/notAI-tech/NudeNet | `c15d8273adad2d0a92f014cc69ab2d6c311a06777a55545f2c4eb46f51911f0f` |
| `nsfwjs.tflite` | NSFWJS MobileNet | 10,305,528 | MIT; upstream third-party notices apply | https://github.com/infinitered/nsfwjs | `fa4e982a62376f65982cf88edeb24d4fd458834dad9c2665c383633eaa079444` |
| `falconsai.onnx` | Falconsai ViT Base | 343,327,085 | Apache-2.0 | https://huggingface.co/Falconsai/nsfw_image_detection | `68ba937a7a9336a5216004002fa35afa82a7e4b6f304ff963d0466b4811d65fd` |

NudeNet is AGPL-3.0: its source is at the upstream link above.
