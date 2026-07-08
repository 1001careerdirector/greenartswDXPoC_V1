# PROJECT_CONTEXT

## Project Role

- Project: `greenartswDXPoC_V1`
- External title: `AI 전환기, 교육운영을 다시 설계하다`
- Role: Google Sites에서 접근하는 교육운영 DX/AX PoC 허브
- Purpose: Google Sites + GitHub Pages + Google Drive 연결 구조를 실험하고, 하위 PoC 화면을 한 곳에서 시연한다.

## Access Structure

- Institution-facing entry: Google Sites
- Demo runtime: GitHub Pages
- Document and artifact storage: Google Drive
- Current GitHub Pages URL: https://1001careerdirector.github.io/greenartswDXPoC_V1/
- Google Sites edit URL: https://sites.google.com/d/1yQetmqs-TDrwQiCRrS8m9XCV5bDqSUuI/p/1MCtSBak5bKhax0NwdveeycxrB08SRYSW/edit?pli=1
- Google Sites published URL: https://sites.google.com/view/dx-poc

## Connected Projects

- `greenartswSC_V1`: 통합 스케줄 대시보드
- `greenartswTEST_V1`: 현장평가준비 진척도 대시보드
- `greenartswDS_V1`: 디자인시스템

## Current Screen Decisions

- The DXPoC screen is a single `index.html` page for GitHub Pages.
- No visible title, subtitle, card container, or page background is shown.
- Button order is:
  1. 통합 스케줄 대시보드
  2. 현장평가준비 진척도 대시보드
  3. 디자인시스템
- Explanatory text, URL display, and new-window button were removed to keep the embed screen clean.
- The screen is now an entry-button hub instead of an embedded viewer.
- Each button opens the corresponding GitHub Pages project with `window.open()`, with same-frame fallback if the popup is blocked.
- The Google Sites embed should show only three top entry buttons on a transparent background.

## Operating Rule

- Use this file as the durable context handoff file for this project.
- When important decisions, URLs, deployment changes, or module roles change, update this file.
- If work continues from another PC, home, office, or laptop, read this file first before changing the project.
- For cross-project work, read each project's own `PROJECT_CONTEXT.md` and synthesize the module context in `greenartswDXPoC_V1`.

## Next Context Files To Create

- `greenartswSC_V1/PROJECT_CONTEXT.md`
- `greenartswTEST_V1/PROJECT_CONTEXT.md`
- `greenartswDS_V1/PROJECT_CONTEXT.md`

## Update Log

- 2026-07-08: Created DXPoC hub screen and deployed it to GitHub Pages.
- 2026-07-08: Established `PROJECT_CONTEXT.md` as the standard cross-device project context file.
- 2026-07-08: Embedded the DXPoC GitHub Pages URL in Google Sites and published the site.
- 2026-07-08: Compressed the DXPoC screen for Google Sites iframe embedding.
- 2026-07-08: Changed the DXPoC slide screen from nested iframe demos to three project entry buttons.
- 2026-07-08: Updated the external concept copy to `AI 전환기, 교육운영을 다시 설계하다`.
- 2026-07-08: Removed visible title, rounded card container, and background; kept only three transparent-embed entry buttons.
- 2026-07-08: Changed entry links to JavaScript buttons because Google Sites iframe embedding can make `target="_blank"` links unreliable.
