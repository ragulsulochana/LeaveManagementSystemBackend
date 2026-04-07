# Modern SaaS UI Redesign Plan (Approved)

## Overview
Redesign LeaveMS frontend to Linear/Stripe/Notion-style: cards, blue gradients, rounded-2xl, shadows-xl, Inter font, responsive.

## Breakdown Steps (Sequential):

### 1. Global Setup ✅
- [x] Update `tailwind.config.js`: Add Inter font, custom colors (#F8FAFC bg, status greens/yellows/reds).
- [x] Edit `main.jsx`: Remove MUI ThemeProvider/CssBaseline (Tailwind only).
- Test: `npm run dev`

**Progress**: 1/7 complete. Next: UI Components."

### 2. UI Components ✅
- [x] Enhance `ui/Button.tsx`: Primary (bg-gradient-blue hover:scale-105), secondary/ghost.
- [x] `ui/Card.tsx`: rounded-2xl shadow-soft hover:shadow-xl.
- [x] `ui/Badge.tsx`: Color-coded with custom theme colors.
- [ ] New: `ui/Chart.tsx` (SVG donut/bar), `ui/Modal.tsx`, `ui/Spinner.tsx`.

**Progress**: 3/7 complete. Next: Dashboard Redesigns (Student first). Charts/Modal/Spinner created."

### 3. Layout ✅
- [x] `DashboardShell.tsx`: Gradient logo, sidebar hovers, navbar effects.

### 4. Dashboard Redesigns (one-by-one)
- [ ] **Student**

### 4. Dashboard Redesigns (one-by-one)
- [x] **Student** ✅: Blue gradient hero, KPI grid.
- [x] **Staff** ✅: Emerald gradient hero, icon KPIs.
- [x] **HOD** ✅: Indigo analytics hero, ChartDonut KPI.
- [x] **Principal** ✅: Slate executive hero, dramatic icon KPIs.

**Progress**: 6/7 complete. Next: Polish & Completion. All dashboards redesigned with modern SaaS UI."

**Progress**: 4.5/7 complete. Next: HOD Dashboard."

**Progress**: 4/7 complete. Next: Staff Dashboard."

### 5. Auth Pages
- [ ] Match split layout exactly (preserve if good).

### 6. Polish
- [ ] Transitions (duration-200), empty states, loading spinners.
- [ ] Responsive: Mobile sidebar collapse.
- [ ] Test: `npm run dev`, all roles/routes.

### 7. Completion
- Update README.md with new screenshots/commands.

**Progress**: 0/7 complete. Next: Global setup."

