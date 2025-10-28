=== TokenLink WebP Converter ===
Contributors: mailborder
Tags: webp, image optimization, media library, imagick, gd
Requires at least: 5.0
Tested up to: 6.8
Stable tag: 1.2.2
License: GPL v3 or later
License URI: https://www.gnu.org/licenses/gpl-3.0.html

Convert JPG and PNG images to .webp directly from the Media Library — quick, secure, and lightweight. Works with Imagick or GD.

== Description ==

**TokenLink WebP Converter** adds one-click controls to the Media Library so you can:
- Create `.webp` versions of existing `.jpg` and `.png` images
- Delete the original images after conversion (optional)
- Automatically register generated `.webp` files in the Media Library

No content rewrites, no background daemons, and no heavy frameworks — this plugin operates entirely within WordPress core standards.

### Features
- ✅ Uses **Imagick** if available, with GD fallback
- ✅ Single-file plugin — lightweight and portable
- ✅ No JavaScript or CSS dependencies
- ✅ Secure AJAX requests with nonces
- ✅ Configurable WebP quality (default 82)
- ✅ Optional thumbnail conversion

### Security
- All AJAX operations are nonce-protected.
- Only authenticated users with proper permissions can trigger conversions or deletions.
- No filesystem writes outside of WordPress uploads.

### Ideal For
- Site owners who want to convert existing images to `.webp` without altering post content or URLs.
- Developers seeking a clean, auditable alternative to complex optimization suites.

== Installation ==

There are three ways to install **TokenLink WebP Converter**:

= 1. From the WordPress Plugin Directory =
1. In your WordPress admin panel, go to **Plugins → Add New**.
2. Search for “TokenLink WebP Converter”.
3. Click **Install Now**, then **Activate**.

= 2. Upload the ZIP file manually =
1. Download the latest release from [GitHub](https://github.com/jcbenton/tokenlink-webp-converter).
2. In WordPress, go to **Plugins → Add New → Upload Plugin**.
3. Choose the downloaded ZIP file and click **Install Now**.
4. After installation, click **Activate Plugin**.

= 3. Copy the plugin manually =
1. Download or clone the repository from [GitHub](https://github.com/jcbenton/tokenlink-webp-converter).
2. Extract and upload the `tokenlink-webp-converter` folder to `/wp-content/plugins/`.
3. In WordPress, navigate to **Plugins → Installed Plugins** and activate **TokenLink WebP Converter**.

Once activated:
1. Go to **Settings → TokenLink WebP** to configure WebP quality and options.
2. Open any image in the Media Library and click **“Create .webp”** to generate WebP versions.

More details and documentation:
👉 [https://www.mailborder.com/tokenlink-webp-converter/](https://www.mailborder.com/tokenlink-webp-converter/)

== Frequently Asked Questions ==

= Does this plugin rewrite image URLs or modify post content? =
No. It only generates and registers `.webp` images. Your posts, pages, and HTML remain untouched.

= Where are the WebP images stored? =
In the same directory as the original image (e.g., `/uploads/2025/10/image.webp`).

= Can I safely delete the original files? =
Yes. The **Delete Original** button is available only when a valid `.webp` version exists. It requires double-click confirmation.

= Do I need Imagick installed? =
No. The plugin automatically falls back to the GD library if Imagick is unavailable.

= Will this affect new uploads? =
No. TokenLink WebP Converter only acts on existing media items that you manually convert.

== Screenshots ==
1. **Media Library Integration** — Create and delete WebP files from the image details screen.
2. **Settings Page** — Configure WebP quality and whether to include thumbnails.

== Changelog ==

= 1.2.2 =
* Added full in-admin AJAX integration for Create/Delete operations.
* Added dynamic UI refresh and double-click confirmation for deletions.
* Added detailed documentation and security hardening.

= 1.2.0 =
* Introduced Create/Delete controls in the Media Library.
* Added AJAX processing and nonce validation.

= 1.0.1 =
* Initial plugin scaffold generated using TokenLink Constructor.

== Upgrade Notice ==

= 1.2.2 =
Improved admin UI, safety checks, and WebP registration in Media Library.