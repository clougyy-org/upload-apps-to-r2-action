# 📤 Upload to Cloudflare R2 Action

A reusable GitHub Action to upload files to Cloudflare R2 storage with organized path structure.

## 🚀 Usage

```yaml
- name: Upload APK to R2
  uses: your-org/upload-to-r2-action@v1
  with:
    filepath: ./app-release.apk
    appname: device-supervision
    apptype: android
    r2-endpoint: ${{ secrets.R2_ENDPOINT }}
    r2-access-key-id: ${{ secrets.R2_ACCESS_KEY_ID }}
    r2-secret-access-key: ${{ secrets.R2_SECRET_ACCESS_KEY }}
    r2-bucket: ${{ secrets.R2_BUCKET }}
    make-public: true