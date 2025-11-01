# 1. Clone your repository
git clone https://github.com/YOUR-USERNAME/buthpitiya-lms-storage.git
cd buthpitiya-lms-storage

# 2. Create all folders at once
mkdir -p chat-images news-images stickers teacher-uploads test-images
mkdir -p grade-{6,7,8,9,10,11,12,13}-{A,B,C,D}

# 3. Create .gitkeep files to preserve empty folders
touch chat-images/.gitkeep
touch news-images/.gitkeep
touch stickers/.gitkeep
touch teacher-uploads/.gitkeep
touch test-images/.gitkeep
touch grade-*/.gitkeep

# 4. Create a descriptive README
cat > README.md << 'EOF'
# Buthpitiya M.V LMS - Storage Repository

This repository stores images and media files for the Buthpitiya M.V Learning Management System.

## 📁 Folder Structure

- `chat-images/` - Images shared in group chats
- `news-images/` - News and announcement images
- `stickers/` - Custom sticker packs
- `teacher-uploads/` - Teacher uploaded materials
- `grade-*/` - Grade-specific uploads
- `test-images/` - Testing purposes

## 🔒 Security

This repository is public to allow CDN access via raw.githubusercontent.com.
All uploads are authenticated through the LMS backend.

## 📊 Storage Info

- **Free Tier:** Unlimited storage for public repositories
- **CDN:** Automatic via GitHub's global CDN
- **Access:** Via `https://raw.githubusercontent.com/`

---

**© 2024 Buthpitiya M.V - All Rights Reserved**
EOF

# 5. Commit and push
git add .
git commit -m "Initial folder structure setup"
git push origin main
