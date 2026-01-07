# Milady NFT Assets

This directory contains the Milady NFT collection images and metadata.

## ⚠️ Files Not Included in Repository

Due to the large size (14GB+), the NFT images are **not included** in the Git repository.

## 📥 How to Download

Run the download script to get all 10,000 Milady NFT images:

```bash
# From project root
python scripts/download_milady_nfts.py
```

The script will:
- Download all 10,000 Milady NFT images (~14GB)
- Save metadata for each NFT
- Create an index file (`milady_nfts_index.json`)
- Resume automatically if interrupted

### Download Options

1. **Download all** (0-9999) - Full collection
2. **Test set** (0-9) - First 10 NFTs for testing
3. **Custom range** - Specify start and end IDs
4. **Resume** - Continue from last download

### Directory Structure

After downloading:

```
assets/milady_nfts/
├── images/              # NFT images (milady_0.png, milady_1.png, ...)
├── metadata/            # NFT metadata JSON files
├── milady_nfts_index.json  # Index of all downloaded NFTs
└── README.md            # This file
```

## 💡 Alternative: Use Without Base NFTs

If you only need the meme generator **layers** (hats, glasses, etc.), you don't need to download the base NFT images. The layers are already included in the repository at `assets/milady_layers/`.

## 📚 More Information

- See main [README.md](../../README.md) for full documentation
- Milady Maker: https://www.miladymaker.net/
- Contract: 0x5Af0D9827E0c53E4799BB226655A1de152A425a5
