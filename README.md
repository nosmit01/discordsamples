# discordsamples

### Files
- [README.md](./README.md)
- [hyp3r3.mp4](./hyp3r3.mp4)
- [medidaMetrics.mov](./medidaMetrics.mov)
- [ups1.mov](./ups1.mov)
- [ups2.mov](./ups2.mov)

### Downloading large files

If GitHub can’t preview these files in the browser, you can still download them:

- Direct download links (click or right‑click “Save link as…”):
  - hyp3r3.mp4: https://raw.githubusercontent.com/nosmit01/discordsamples/main/hyp3r3.mp4
  - medidaMetrics.mov: https://raw.githubusercontent.com/nosmit01/discordsamples/main/medidaMetrics.mov
  - ups1.mov: https://raw.githubusercontent.com/nosmit01/discordsamples/main/ups1.mov
  - ups2.mov: https://raw.githubusercontent.com/nosmit01/discordsamples/main/ups2.mov

- Using curl from the command line:

```bash
curl -L -o hyp3r3.mp4 https://raw.githubusercontent.com/nosmit01/discordsamples/main/hyp3r3.mp4
curl -L -o medidaMetrics.mov https://raw.githubusercontent.com/nosmit01/discordsamples/main/medidaMetrics.mov
curl -L -o ups1.mov https://raw.githubusercontent.com/nosmit01/discordsamples/main/ups1.mov
curl -L -o ups2.mov https://raw.githubusercontent.com/nosmit01/discordsamples/main/ups2.mov
```

- If this repo uses Git LFS (Large File Storage), clone and pull LFS objects:

```bash
# Install once (macOS):
brew install git-lfs
git lfs install

git clone --filter=blob:none https://github.com/nosmit01/discordsamples.git
cd discordsamples
git lfs pull --include="hyp3r3.mp4,medidaMetrics.mov,ups1.mov,ups2.mov"
```

- Download only these files (sparse checkout), then pull LFS if needed:

```bash
git clone --filter=blob:none --no-checkout https://github.com/nosmit01/discordsamples.git
cd discordsamples
git sparse-checkout init --cone
git sparse-checkout set hyp3r3.mp4 medidaMetrics.mov ups1.mov ups2.mov
git checkout
# If using LFS:
git lfs pull --include="hyp3r3.mp4,medidaMetrics.mov,ups1.mov,ups2.mov"
```

Tip: For very large assets, attaching them to a GitHub Release is often the most reliable experience.