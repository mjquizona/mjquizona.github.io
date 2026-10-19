MJ portfolio — GitHub Pages
Publish
Extract this ZIP first. Upload the extracted files, NOT the ZIP.
Create a PUBLIC GitHub repository named YOURUSERNAME.github.io (replace YOURUSERNAME with your actual GitHub username). This gives you https://YOURUSERNAME.github.io. If that repository already exists, use a new repository named mj-portfolio instead; its address will be https://YOURUSERNAME.github.io/mj-portfolio/.
In the repository, choose Add file > Upload files. Drag in all extracted files AND the assets folder. Keep index.html at the repository root, not inside another folder. Commit the upload to main. You can upload assets in smaller batches if your connection struggles.
Open Settings > Pages. Under Build and deployment, choose Deploy from a branch, then main and / (root), and Save.
Wait for deployment, then use Visit site. Check the videos and contact links on desktop and phone.
The .nojekyll file is included. Ensure it uploads too; if your file picker hides it, create an empty file named .nojekyll directly in the repository.
GitHub supplies a free github.io address, not a separately registered custom domain. Your repository and portfolio media will be public. No upload or deployment was performed while creating this package.
Official instructions:
https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository
Contact form — setup still required
The direct email link works. Automated form delivery is NOT connected or tested yet, and Send inquiry stays disabled until configured.
Create a form in your own Formspree account: https://formspree.io/
Set mjquizona@gmail.com as its notification recipient and complete email verification.
Copy the public endpoint from the dashboard (https://formspree.io/f/ followed by your form ID).
Edit config.js and paste that endpoint inside the empty formEndpoint quotes. Do not add passwords, account tokens, or private API keys.
Commit the change. Submit a test on the published website, check the Formspree dashboard, and verify receipt in mjquizona@gmail.com, including Spam. Only then consider delivery operational.
The form validates fields, sends a real POST, and reports success only after service confirmation. Failed requests retain the message. Use the provider's spam settings and check its current submission limits and pricing. GitHub Pages only hosts the frontend; Formspree handles email.
Included files
index.html: page content
styles.css: appearance and responsive layouts
app.js: filters, video player, contact submission
portfolio.js: video titles, categories, paths, durations
config.js: public form endpoint
favicon.svg: site icon
.nojekyll: static publishing configuration
assets/: 13 optimized MP4 videos, 13 matching poster frames, and MJ's profile photo
The Cloudflare-only _headers file is omitted because GitHub Pages does not apply it. All site asset links are relative, so both repository URL styles work. No dependencies or build command are required. Originals and the resume are not included; originals remain untouched.
Update your work
Replace a video/poster in assets and update its entry in portfolio.js. To add or remove a sample, add or remove its entry and corresponding assets. Use unique IDs. The four initial picks are listed in the selected array near the top of app.js. If changing the number of samples, also update the filter counts and View all label in index.html. Use H.264/AAC MP4 files with fast-start enabled and portrait WebP posters.
Verification
The package was checked for archive integrity, all 13 video/poster references, profile image, and required source files. Every included video is under GitHub's 25 MiB browser-upload limit. Full browser/mobile playback, live deployment, and email delivery have not been verified. Review those after publishing. The videos load only when selected for playback.
