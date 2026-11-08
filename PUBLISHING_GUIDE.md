# Publication & Hosting Guide — no fabricated links

The Excel model, PDFs and PowerPoint are created locally in this package. **No GitHub, Google Drive, Notion or LinkedIn account has been accessed or published to.** You must publish the repository yourself (or explicitly authorise an available integration) to generate a real public URL.

## Recommended workflow (GitHub + native LinkedIn PDF)

1. **Prepare the public files.** Verify `model/Dominos_LBO_Financial_Model.xlsx` opens and that the `Checks` sheet reads `PASS`. Open all PDFs and the PPTX. Read the investment memo’s assumptions and company-boundary caveat. Do **not** add your personal CV, email/phone number or the uploaded US DPZ filings to the public repository.
2. Visit https://github.com/new while logged in. Choose a clear name such as `dominos-uk-lbo-analysis` (illustrative *name*, not a purported live URL); select **Public**, and create the repository. Do not auto-add README if importing the prepared folder contents into an empty repository.
3. Extract `Dominos_GitHub_Repository.zip`. In the new repo use **Add file → Upload files**, drag in the contents of the extracted repository (preserving `model/`, `documents/`, `slides/`, `linkedin/`, `sources/`), commit. For multi-folder drag/drop, use GitHub Desktop or `git` command line if the browser upload does not preserve folders. Confirm README links work.
4. Copy the **actual** GitHub repository address from the browser. Replace `[PROJECT_URL]` in `linkedin/Dominos_LinkedIn_Post.md`; do not use `https://github.com/username/...` as if it exists. Optionally update README with the actual project landing-page link.
5. On LinkedIn, choose **Start a post → Add a document** and upload `linkedin/Dominos_LinkedIn_Carousel.pdf`. Paste the corrected English post. Verify preview and figures before publishing; add the *real* GitHub URL. Prefer a native carousel plus repository link rather than linking to your raw Excel file alone.
6. On your LinkedIn profile, add the GitHub repository to **Featured**, using the title and summary in `linkedin/Dominos_CV_and_LinkedIn_Project_Description.md`. Add an **Independent Projects** entry only if fully able to explain your work.
7. Open the public repository in a signed-out/incognito window, test direct PDF / Excel links and spelling. If a link fails, fix it before sharing with recruiters.

## Google Drive / Notion alternatives

- **Google Drive:** Upload the finished files and set each intended public item to **General access → Anyone with the link → Viewer**. This is useful for easy downloads but less transparent about version history than GitHub. Verify using a signed-out browser. Do not share edit permissions.
- **Notion:** Publish a landing page with the thesis and external GitHub or Google Drive file links. Helpful for a polished visual portfolio, but a GitHub README alone is sufficient. Do not create a Notion link until the page is actually published.
- **GitHub:** Recommended home for source references, model version history, transparent assumptions and downloads. Binary Excel and PowerPoint cannot be inspected line-by-line on GitHub, so add descriptions and methodology in README.

## Final posting quality gates

- The target entity on *every* page is **Domino’s Pizza Group plc (LSE: DOM)**, not US DPZ.
- The information date is **6 Nov 2026**, financial latest audited FY2025, unaudited H1 2026, qualitative Q3 2026.
- The takeover price and 30% premium are explicitly hypothetical.
- Exit returns are **gross sponsor returns**, not guaranteed outcomes or net LP cash flows.
- The memo, PPTX, carousel and LinkedIn text all show approximately **7.5% IRR**, **1.44x MOIC**, **£1,445.9m entry EV** and **£707.1m maximum equity price** at 20% required return.
- No personally identifying information is placed in a public file by accident.

## Optional GitHub command-line publishing (after creating your account/repository)

```bash
cd path/to/extracted/repo
# Initialize and commit locally
git init
git add .
git commit -m "Initial independent DPG LBO project"
# Set the actual repository URL you created, not a placeholder
git remote add origin REAL_GIT_REMOTE_URL
git branch -M main
git push -u origin main
```

This package does not contain a fabricated public URL or proof of a published post. You control publication and public accessibility.
