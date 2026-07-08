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
  4. 프로젝트1 성과 리포트(Admin)
  5. 프로젝트1 훈련생 피드백
- Explanatory text, URL display, and new-window button were removed to keep the embed screen clean.
- The screen is now an entry-button hub instead of an embedded viewer.
- Each button opens the corresponding GitHub Pages project with `window.open()` only; same-frame fallback is intentionally disabled so the button hub does not navigate away.
- The field-evaluation button opens `greenartswTEST_V1/channel_Dashboard.html` directly so the Google Drive course-space view appears without depending on the repo root redirect.
- The Google Sites embed should show only top entry buttons on a transparent background.
- Google Sites controls the outer iframe height; the GitHub Pages child cannot reliably auto-resize the parent iframe. Keep the DXPoC hub as a compact one-row button strip and avoid breakpoint rules that turn the buttons into tall vertical stacks.
- Project1 buttons use a different color level so they read as a lower-level case/project group.
- The Project1 performance report button opens a DXPoC-owned admin launcher page (`project1-admin.html`) so the hidden 2026biz1 controls can be handled without editing the public 2026biz1 source before company feedback is complete.

## Future Implementation Notes

- Keep the current `project1-admin.html` wrapper approach until company feedback on the public `2026biz1` page is complete.
- After company feedback is confirmed, move the student/view/theme controls into `2026biz1` as an official Admin mode instead of continuing the wrapper-only workaround.
- Do not debug or alter the public `2026biz1` source prematurely while company feedback is still pending.

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
- 2026-07-08: Removed same-frame fallback from button clicks because it could navigate the button hub itself.
- 2026-07-08: Added two Project1 buttons for `2026biz1` performance report and trainee feedback, with a distinct color level.
- 2026-07-08: Added `project1-admin.html` as a workaround launcher for student/view/theme controls without modifying the public `2026biz1` page.
- 2026-07-08: Recorded the future plan to formalize the wrapper controls as a native `2026biz1` Admin mode only after company feedback is complete.
- 2026-07-08: Pointed the field-evaluation entry button directly to `greenartswTEST_V1/channel_Dashboard.html` for the Google Drive course-space dashboard view.
- 2026-07-08: Adjusted the DXPoC hub button strip for Google Sites iframe embedding: removed the tall one-column mobile breakpoint, made button sizing fluid, and switched very narrow screens to a horizontal strip.
