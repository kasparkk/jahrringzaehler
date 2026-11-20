# Jahrringzähler / Tree Ring Counter

Installable web app: photograph a stump or disc, tap the centre and the bark, and the tree rings along that line are counted. Wrong or missing rings can be fixed by tapping.

- Classic detection: edge profile along 37 rays, rings traced from ray to ray (idea from CS-TRD).
- AI detection (optional): U-Net (ResNet18) fine-tuned from DeepCS-TRD (MIT) on UruDendro2 (CC BY 4.0) and the Purdue hardwood growth-ring dataset (MIT). Runs on the device with TensorFlow.js; the model (`ring_model.bin`, int8) is downloaded once.
- Several directions: count along 3–4 radii and use the middle value.
- Works offline after the first visit (service worker).

Open: https://kasparkk.github.io/jahrringzaehler/

## Licence

MIT, see [LICENSE](LICENSE). The AI model builds on DeepCS-TRD (MIT), UruDendro2 (CC BY 4.0) and the Purdue hardwood growth-ring dataset (MIT), credited above.
