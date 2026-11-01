# CodeTest
<!DOCTYPE html>

<html lang="en"><head>
<meta charset="utf-8"/>
<meta content="width=device-width, initial-scale=1.0" name="viewport"/>
<title>CareShift &amp; Pay - Digital Payslip Generator &amp; Archive</title>
<!-- Material Symbols Outlined -->
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap" rel="stylesheet"/>
<!-- Fonts: Manrope & JetBrains Mono -->
<link href="https://fonts.googleapis.com" rel="preconnect"/>
<link crossorigin="" href="https://fonts.gstatic.com" rel="preconnect"/>
<link href="https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@400;500;600;700&amp;family=Manrope:wght@400;500;600;700;800&amp;display=swap" rel="stylesheet"/>
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap" rel="stylesheet"/>
<!-- Tailwind CSS -->
<script src="https://cdn.tailwindcss.com?plugins=forms,container-queries"></script>
<script id="tailwind-config">
    tailwind.config = {
      darkMode: "class",
      theme: {
        extend: {
          "colors": {
            "on-secondary": "#ffffff",
            "on-primary-fixed": "#0d1d2a",
            "inverse-surface": "#2d3133",
            "secondary-fixed": "#89f5e7",
            "surface-container": "#eceef0",
            "on-error": "#ffffff",
            "inverse-primary": "#b8c8da",
            "on-secondary-fixed": "#00201d",
            "on-secondary-container": "#006f66",
            "on-background": "#191c1e",
            "on-tertiary-fixed": "#001d31",
            "surface-container-high": "#e6e8ea",
            "secondary": "#006a61",
            "on-tertiary": "#ffffff",
            "primary-fixed": "#d4e4f6",
            "tertiary-fixed": "#cce5ff",
            "surface-variant": "#e0e3e5",
            "on-tertiary-container": "#1d8cd0",
            "on-surface-variant": "#43474c",
            "tertiary-container": "#002035",
            "on-primary-container": "#778797",
            "secondary-container": "#86f2e4",
            "inverse-on-surface": "#eff1f3",
            "error": "#ba1a1a",
            "on-error-container": "#93000a",
            "on-surface": "#191c1e",
            "on-tertiary-fixed-variant": "#004b73",
            "background": "#f7f9fb",
            "surface-container-low": "#f2f4f6",
            "error-container": "#ffdad6",
            "surface-container-highest": "#e0e3e5",
            "primary-fixed-dim": "#b8c8da",
            "secondary-fixed-dim": "#6bd8cb",
            "on-primary": "#ffffff",
            "surface-dim": "#d8dadc",
            "primary": "#00040a",
            "tertiary": "#00050b",
            "tertiary-fixed-dim": "#93ccff",
            "on-primary-fixed-variant": "#394857",
            "primary-container": "#0f1f2c",
            "outline": "#74777c",
            "outline-variant": "#c4c7cc",
            "on-secondary-fixed-variant": "#005049",
            "surface-bright": "#f7f9fb",
            "surface": "#f7f9fb",
            "surface-tint": "#50606f",
            "surface-container-lowest": "#ffffff"
          },
          "borderRadius": {
            "DEFAULT": "0.25rem",
            "lg": "0.5rem",
            "xl": "0.75rem",
            "full": "9999px"
          },
          "spacing": {
            "gutter-desktop": "1.5rem",
            "margin-desktop": "3rem",
            "space-xl": "1.5rem",
            "margin-tablet": "2rem",
            "space-md": "0.75rem",
            "space-sm": "0.5rem",
            "gutter": "1rem",
            "space-2xl": "2rem",
            "space-lg": "1rem",
            "gutter-tablet": "1.25rem",
            "margin": "1rem",
            "space-xs": "0.25rem"
          },
          "fontFamily": {
            "label-md": ["Manrope"],
            "label-lg": ["Manrope"],
            "label-sm": ["Manrope"],
            "data-time": ["JetBrains Mono"],
            "data-currency-md": ["JetBrains Mono"],
            "headline-lg": ["Manrope"],
            "headline-md": ["Manrope"],
            "display-lg": ["Manrope"],
            "body-sm": ["Manrope"],
            "data-currency-lg": ["JetBrains Mono"],
            "headline-sm": ["Manrope"],
            "body-md": ["Manrope"],
            "display-lg-mobile": ["Manrope"],
            "body-lg": ["Manrope"]
          },
          "fontSize": {
            "label-md": ["12px", { "lineHeight": "16px", "letterSpacing": "0.02em", "fontWeight": "600" }],
            "label-lg": ["14px", { "lineHeight": "20px", "letterSpacing": "0.01em", "fontWeight": "600" }],
            "label-sm": ["11px", { "lineHeight": "14px", "letterSpacing": "0.03em", "fontWeight": "500" }],
            "data-time": ["13px", { "lineHeight": "18px", "letterSpacing": "0em", "fontWeight": "500" }],
            "data-currency-md": ["18px", { "lineHeight": "24px", "letterSpacing": "-0.02em", "fontWeight": "500" }],
            "headline-lg": ["24px", { "lineHeight": "32px", "letterSpacing": "-0.01em", "fontWeight": "700" }],
            "headline-md": ["20px", { "lineHeight": "28px", "letterSpacing": "-0.005em", "fontWeight": "600" }],
            "display-lg": ["36px", { "lineHeight": "44px", "letterSpacing": "-0.02em", "fontWeight": "700" }],
            "body-sm": ["12px", { "lineHeight": "16px", "fontWeight": "400" }],
            "data-currency-lg": ["28px", { "lineHeight": "32px", "letterSpacing": "-0.03em", "fontWeight": "600" }],
            "headline-sm": ["18px", { "lineHeight": "24px", "fontWeight": "600" }],
            "body-md": ["14px", { "lineHeight": "20px", "fontWeight": "400" }],
            "display-lg-mobile": ["28px", { "lineHeight": "36px", "letterSpacing": "-0.01em", "fontWeight": "700" }],
            "body-lg": ["16px", { "lineHeight": "24px", "fontWeight": "400" }]
          }
        },
      },
    }
  </script>
<style>
    body {
      min-height: max(884px, 100dvh);
    }
  </style>
  </head>
<body class="bg-background text-on-surface antialiased min-h-screen selection:bg-secondary-container selection:text-on-secondary-container pb-28">
<!-- TOP APP BAR (from Shared Components JSON) -->
<header class="fixed top-0 left-0 w-full z-40 flex justify-between items-center px-margin h-14 bg-surface-container-lowest dark:bg-surface-container-low shadow-[0_2px_8px_-2px_rgba(15,31,44,0.05)]">
<div class="flex items-center gap-3">
<div class="w-8 h-8 rounded-full overflow-hidden border border-outline-variant bg-surface-container flex items-center justify-center shrink-0">
<img class="w-full h-full object-cover" data-alt="Close up professional portrait of a British female NHS community health care worker in a soft jade scrub uniform with hospital ID badge and gentle smile, bathed in warm clinical morning light with serene subtle neutral backdrop." src="https://lh3.googleusercontent.com/aida-public/AB6AXuDXaX7nRtkODand9tnhfcljQgZjUEi1haoLM5RQ6uNLyurgh7HiytTQ8fcSninYisNBDRbLX0Acgn0eheDjwOg5oD1tjOOR_zVkU0YUu06dQGgd_xP-t6xW-9VOW2GXlVMjxDPY6mQpWrj3dg1qEd3hk_pWRVqNWGeLGOCpsTzOPXE_js1OGA_dVd19Ir7QJ4WHFIFbmG5nmxLq_nZV907ZNM2VApiz66LA_4O7hXQx"/>
</div>
<span class="text-headline-sm font-headline-sm font-bold text-on-surface dark:text-inverse-on-surface tracking-tight">CareShift &amp; Pay</span>
</div>
<div class="flex items-center gap-2">
<button aria-label="Notifications" class="w-9 h-9 flex items-center justify-center rounded-lg hover:bg-surface-container dark:hover:bg-surface-container-high transition-colors text-on-surface-variant active:translate-y-px">
<span class="material-symbols-outlined text-[20px]">notifications</span>
</button>
</div>
</header>
<!-- MAIN CANVAS -->
<main class="pt-20 px-4 md:px-8 max-w-[1120px] mx-auto space-y-6">
<!-- Screen Title & Operational Context -->
<div class="flex flex-col md:flex-row md:items-end md:justify-between gap-3 pb-2">
<div>
<div class="flex items-center gap-2 mb-1">
<span class="inline-flex items-center px-2 py-0.5 rounded-full text-label-sm font-label-sm bg-[#CCFBF1] text-[#0F766E] border border-[#99F6E4]">
<span class="w-1.5 h-1.5 rounded-full bg-[#0D9488] mr-1.5 animate-pulse"></span>
            Verified HMRC &amp; RTI Compliant
          </span>
<span class="text-label-sm font-label-sm text-on-surface-variant">Tax Year 2024/25</span>
</div>
<h1 class="text-headline-lg font-headline-lg text-primary tracking-tight">Digital Payslip Generator &amp; Archive</h1>
<p class="text-body-md font-body-md text-on-surface-variant">Review live shift calculations, deductions breakdown, and download verified wage slips.</p>
</div>
<!-- Quick Sync Action -->
<button class="self-start md:self-auto inline-flex items-center gap-2 px-3.5 py-2 rounded-lg bg-surface-container-lowest border border-outline-variant hover:bg-surface-container text-on-surface font-label-md text-label-md active:translate-y-px transition-all">
<span class="material-symbols-outlined text-[16px] text-secondary">sync</span>
<span>Regenerate from Live Hours</span>
</button>
</div>
<!-- Period Selector (Segmented Control & Custom Picker) -->
<div class="bg-surface-container-lowest rounded-xl p-2 border border-outline-variant shadow-sm flex flex-col md:flex-row items-stretch md:items-center justify-between gap-2">
<div class="inline-flex p-1 bg-surface-container rounded-lg gap-1 overflow-x-auto">
<button class="px-3.5 py-1.5 rounded-md text-label-md font-label-md bg-surface-container-lowest text-on-surface shadow-sm font-semibold whitespace-nowrap transition-all">
          February 2025 (Current)
        </button>
<button class="px-3.5 py-1.5 rounded-md text-label-md font-label-md text-on-surface-variant hover:text-on-surface whitespace-nowrap transition-colors">
          January 2025
        </button>
<button class="px-3.5 py-1.5 rounded-md text-label-md font-label-md text-on-surface-variant hover:text-on-surface whitespace-nowrap transition-colors">
          December 2024
        </button>
</div>
<div class="flex items-center gap-2 px-2">
<button class="inline-flex items-center gap-1.5 px-3 py-1.5 rounded-lg border border-outline-variant bg-surface-container-lowest text-on-surface-variant hover:text-on-surface text-label-md font-label-md active:translate-y-px transition-all">
<span class="material-symbols-outlined text-[18px]">calendar_today</span>
<span>Custom Date Range</span>
<span class="material-symbols-outlined text-[16px]">expand_more</span>
</button>
</div>
</div>
<!-- DIGITAL PAYSLIP DOCUMENT PREVIEW -->
<div class="bg-surface-container-lowest border border-outline-variant rounded-2xl p-4 sm:p-6 md:p-8 shadow-[0_8px_24px_-4px_rgba(15,31,44,0.08),0_2px_6px_-1px_rgba(15,31,44,0.04)] relative">
<!-- Watermark / Security Strip Accent -->
<div class="absolute top-0 left-0 right-0 h-1.5 bg-gradient-to-r from-secondary via-secondary-container to-secondary rounded-t-2xl"></div>
<!-- Payslip Header: Employer & Employee Metadata -->
<div class="flex flex-col lg:flex-row lg:items-start justify-between gap-6 pb-6 border-b border-outline-variant">
<div class="space-y-1.5">
<div class="flex items-center gap-2">
<span class="material-symbols-outlined text-secondary text-[24px]">local_hospital</span>
<span class="text-headline-md font-headline-md text-primary font-bold">CareFirst Healthcare Trust Ltd</span>
</div>
<p class="text-body-sm font-body-sm text-on-surface-variant">St Jude Ward, NHS Bank Partnership &amp; Overtime Rota</p>
<div class="flex items-center gap-2 pt-1">
<span class="px-2 py-0.5 rounded-full text-label-sm font-label-sm bg-[#EDE9FE] text-[#5B21B6] border border-[#DDD6FE]">
              Payroll Period: 11
            </span>
<span class="text-label-sm font-label-sm text-on-surface-variant">BACS Payment Standard</span>
</div>
</div>
<!-- Inset Grid for Employee Specifics -->
<div class="grid grid-cols-2 sm:grid-cols-3 gap-3 bg-surface-container-low p-3.5 rounded-xl border border-outline-variant/60">
<div>
<div class="text-label-sm font-label-sm text-on-surface-variant">Employee</div>
<div class="text-body-md font-body-md font-semibold text-on-surface">Sarah Jenkins</div>
<div class="text-body-sm font-body-sm text-on-surface-variant font-data-time">PIN: CW-89211</div>
</div>
<div>
<div class="text-label-sm font-label-sm text-on-surface-variant">Tax Code / NI No</div>
<div class="text-body-md font-body-md font-semibold text-on-surface">1257L</div>
<div class="text-body-sm font-body-sm text-on-surface-variant font-data-time">QQ 12 34 56 A</div>
</div>
<div class="col-span-2 sm:col-span-1">
<div class="text-label-sm font-label-sm text-on-surface-variant">Pay Date</div>
<div class="text-body-md font-body-md font-semibold text-secondary">28 Feb 2025</div>
<div class="text-body-sm font-body-sm text-on-surface-variant">Monthly Cycle</div>
</div>
</div>
</div>
<!-- Financial Ledger Bento: Earnings vs Deductions -->
<div class="grid grid-cols-1 lg:grid-cols-12 gap-6 my-6">
<!-- Column 1: Itemized Earnings (7 Cols) -->
<div class="lg:col-span-7 space-y-4">
<div class="flex items-center justify-between pb-1 border-b border-outline-variant">
<h2 class="text-headline-sm font-headline-sm text-primary flex items-center gap-1.5">
<span class="material-symbols-outlined text-secondary text-[20px]">payments</span>
              Itemized Earnings
            </h2>
<span class="text-label-sm font-label-sm text-on-surface-variant">Calculated from Ward Logs</span>
</div>
<!-- Table Container -->
<div class="overflow-x-auto">
<table class="w-full text-left border-collapse">
<thead>
<tr class="text-label-sm font-label-sm text-on-surface-variant border-b border-surface-container">
<th class="py-2 pr-2 font-medium">Description</th>
<th class="py-2 px-2 text-right font-medium">Units / Hrs</th>
<th class="py-2 px-2 text-right font-medium">Rate</th>
<th class="py-2 pl-2 text-right font-medium">Gross (£)</th>
</tr>
</thead>
<tbody class="divide-y divide-surface-container text-body-md font-body-md">
<tr class="hover:bg-surface-container-low/50">
<td class="py-2.5 pr-2">
<div class="font-medium text-on-surface">Standard Hours</div>
<div class="text-body-sm font-body-sm text-on-surface-variant">Core contracted hours</div>
</td>
<td class="py-2.5 px-2 text-right font-data-time text-data-time">140.0 hrs</td>
<td class="py-2.5 px-2 text-right font-data-time text-data-time">£16.80</td>
<td class="py-2.5 pl-2 text-right font-data-currency-md text-data-currency-md text-on-surface font-semibold">£2,352.00</td>
</tr>
<tr class="hover:bg-surface-container-low/50">
<td class="py-2.5 pr-2">
<div class="font-medium text-on-surface flex items-center gap-1.5">
<span>Night Enhancement Uplift</span>
<span class="px-1.5 py-0.2 rounded text-[10px] bg-[#EDE9FE] text-[#5B21B6] border border-[#DDD6FE]">Night</span>
</div>
<div class="text-body-sm font-body-sm text-on-surface-variant">20:00 - 08:00 Ward rate</div>
</td>
<td class="py-2.5 px-2 text-right font-data-time text-data-time">34.5 hrs</td>
<td class="py-2.5 px-2 text-right font-data-time text-data-time">£5.04</td>
<td class="py-2.5 pl-2 text-right font-data-currency-md text-data-currency-md text-on-surface font-semibold">£173.88</td>
</tr>
<tr class="hover:bg-surface-container-low/50">
<td class="py-2.5 pr-2">
<div class="font-medium text-on-surface">Weekend Premium</div>
<div class="text-body-sm font-body-sm text-on-surface-variant">Saturday &amp; Sunday shifts</div>
</td>
<td class="py-2.5 px-2 text-right font-data-time text-data-time">23.0 hrs</td>
<td class="py-2.5 px-2 text-right font-data-time text-data-time">£5.04</td>
<td class="py-2.5 pl-2 text-right font-data-currency-md text-data-currency-md text-on-surface font-semibold">£115.92</td>
</tr>
<tr class="hover:bg-surface-container-low/50">
<td class="py-2.5 pr-2">
<div class="font-medium text-on-surface">Sleep-in Shift Allowance</div>
<div class="text-body-sm font-body-sm text-on-surface-variant">Residential overnight duty</div>
</td>
<td class="py-2.5 px-2 text-right font-data-time text-data-time">2 nights</td>
<td class="py-2.5 px-2 text-right font-data-time text-data-time">£45.00</td>
<td class="py-2.5 pl-2 text-right font-data-currency-md text-data-currency-md text-on-surface font-semibold">£90.00</td>
</tr>
<tr class="hover:bg-surface-container-low/50">
<td class="py-2.5 pr-2">
<div class="font-medium text-on-surface flex items-center gap-1.5">
<span>Mileage Reimbursement</span>
<span class="px-1.5 py-0.2 rounded text-[10px] bg-surface-container-high text-on-surface-variant">Non-taxable</span>
</div>
<div class="text-body-sm font-body-sm text-on-surface-variant">Community domiciliary visits</div>
</td>
<td class="py-2.5 px-2 text-right font-data-time text-data-time">84 miles</td>
<td class="py-2.5 px-2 text-right font-data-time text-data-time">£0.45</td>
<td class="py-2.5 pl-2 text-right font-data-currency-md text-data-currency-md text-on-surface font-semibold">£37.80</td>
</tr>
</tbody>
</table>
</div>
<!-- Total Gross Card -->
<div class="flex items-center justify-between p-3.5 rounded-xl bg-surface-container-low border border-outline-variant">
<span class="text-label-lg font-label-lg text-on-surface font-bold uppercase tracking-wider">Total Gross Pay</span>
<span class="text-data-currency-lg font-data-currency-lg text-primary font-bold">£2,769.60</span>
</div>
</div>
<!-- Column 2: Itemized Deductions (5 Cols) -->
<div class="lg:col-span-5 space-y-4">
<div class="flex items-center justify-between pb-1 border-b border-outline-variant">
<h2 class="text-headline-sm font-headline-sm text-primary flex items-center gap-1.5">
<span class="material-symbols-outlined text-outline text-[20px]">account_balance</span>
              Itemized Deductions
            </h2>
<span class="text-label-sm font-label-sm text-on-surface-variant">Statutory &amp; Pension</span>
</div>
<div class="bg-surface-container-lowest border border-outline-variant rounded-xl divide-y divide-surface-container overflow-hidden">
<div class="p-3 flex items-center justify-between hover:bg-surface-container-low/40">
<div>
<div class="text-body-md font-body-md font-medium text-on-surface">PAYE Income Tax</div>
<div class="text-body-sm font-body-sm text-on-surface-variant">Standard Rate 20% bracket</div>
</div>
<span class="text-data-currency-md font-data-currency-md text-error font-medium">-£298.40</span>
</div>
<div class="p-3 flex items-center justify-between hover:bg-surface-container-low/40">
<div>
<div class="text-body-md font-body-md font-medium text-on-surface">National Insurance</div>
<div class="text-body-sm font-body-sm text-on-surface-variant">Class 1 Primary contributions</div>
</div>
<span class="text-data-currency-md font-data-currency-md text-error font-medium">-£181.20</span>
</div>
<div class="p-3 flex items-center justify-between hover:bg-surface-container-low/40">
<div>
<div class="text-body-md font-body-md font-medium text-on-surface">NHS Pension Scheme</div>
<div class="text-body-sm font-body-sm text-on-surface-variant">Tier 4 Contribution (7.1%)</div>
</div>
<span class="text-data-currency-md font-data-currency-md text-error font-medium">-£196.64</span>
</div>
</div>
<!-- Total Deductions Card -->
<div class="flex items-center justify-between p-3.5 rounded-xl bg-error-container/20 border border-error-container">
<span class="text-label-lg font-label-lg text-error font-bold uppercase tracking-wider">Total Deductions</span>
<span class="text-data-currency-lg font-data-currency-lg text-error font-bold">-£676.24</span>
</div>
<!-- YTD Accrual Summary Mini-well -->
<div class="p-3.5 rounded-xl bg-surface-container-low border border-outline-variant/60 text-body-sm font-body-sm space-y-1">
<div class="text-label-sm font-label-sm text-on-surface-variant font-semibold">YEAR-TO-DATE (YTD) BALANCES</div>
<div class="flex justify-between text-on-surface">
<span>YTD Taxable Gross:</span>
<span class="font-data-time">£29,480.20</span>
</div>
<div class="flex justify-between text-on-surface">
<span>YTD Income Tax:</span>
<span class="font-data-time">£3,184.40</span>
</div>
<div class="flex justify-between text-on-surface">
<span>YTD Employee Pension:</span>
<span class="font-data-time">£2,093.09</span>
</div>
</div>
</div>
</div>
<!-- Net Pay Callout Banner (Hero Inset) -->
<div class="mt-6 rounded-xl bg-primary-container text-on-secondary p-5 md:p-6 flex flex-col md:flex-row items-start md:items-center justify-between gap-4 border border-outline-variant shadow-sm">
<div class="space-y-1">
<span class="text-label-md font-label-md text-secondary-fixed uppercase tracking-wider font-semibold">Official Take-Home Pay</span>
<div class="flex items-baseline gap-2">
<span class="text-label-lg font-label-lg text-on-secondary">NET PAY:</span>
<span class="text-display-lg-mobile md:text-display-lg font-display-lg text-secondary-fixed tracking-tight font-data-currency-lg">£2,093.36</span>
</div>
<div class="flex items-center gap-2 text-body-sm font-body-sm text-surface-container-highest">
<span class="material-symbols-outlined text-[16px] text-secondary-fixed">credit_card</span>
<span>Paid directly into Barclays •••• 4821</span>
<span class="text-outline-variant">•</span>
<span>Settlement Ref: BAC-892-FEB25</span>
</div>
</div>
<div class="flex items-center gap-2 w-full md:w-auto">
<div class="px-3.5 py-2 rounded-lg bg-surface-container-lowest/10 border border-outline-variant/30 text-right w-full md:w-auto">
<div class="text-label-sm font-label-sm text-inverse-primary">Disbursement Status</div>
<div class="text-body-md font-body-md font-semibold text-on-secondary flex items-center gap-1.5 justify-end">
<span class="w-2 h-2 rounded-full bg-secondary-fixed"></span>
              Scheduled on 28 Feb
            </div>
</div>
</div>
</div>
<!-- Action Bar -->
<div class="mt-6 pt-6 border-t border-outline-variant flex flex-wrap items-center justify-between gap-3">
<div class="flex flex-wrap items-center gap-2.5 w-full sm:w-auto">
<!-- Primary: Download PDF Payslip -->
<button class="flex-1 sm:flex-none inline-flex items-center justify-center gap-2 px-5 h-12 rounded-lg bg-[#0D9488] hover:bg-[#0F766E] text-white font-label-lg text-label-lg shadow-sm active:translate-y-px transition-all">
<span class="material-symbols-outlined text-[20px]">download</span>
<span>Download PDF Payslip</span>
</button>
<!-- Secondary: Share / Email -->
<button class="flex-1 sm:flex-none inline-flex items-center justify-center gap-2 px-4 h-12 rounded-lg bg-surface-container-lowest border border-outline-variant hover:bg-surface-container text-on-surface font-label-lg text-label-lg active:translate-y-px transition-all">
<span class="material-symbols-outlined text-[20px] text-on-surface-variant">mail</span>
<span>Share / Email</span>
</button>
</div>
<!-- Sync Outline Action -->
<button class="w-full sm:w-auto inline-flex items-center justify-center gap-2 px-4 h-12 rounded-lg border border-outline text-on-surface hover:bg-surface-container-low font-label-md text-label-md active:translate-y-px transition-all">
<span class="material-symbols-outlined text-[18px]">sync</span>
<span>Regenerate from Live Hours</span>
</button>
</div>
</div>
<!-- ARCHIVE SECTION (Past Payslips) -->
<div class="space-y-3 pt-2">
<div class="flex items-center justify-between">
<div>
<h2 class="text-headline-md font-headline-md text-primary">Payslip Archive</h2>
<p class="text-body-sm font-body-sm text-on-surface-variant">Instant access to verified prior periods and download receipts</p>
</div>
<button class="text-label-md font-label-md text-secondary hover:underline flex items-center gap-1">
<span>View All Years</span>
<span class="material-symbols-outlined text-[16px]">chevron_right</span>
</button>
</div>
<!-- Archive Cards Grid -->
<div class="grid grid-cols-1 md:grid-cols-3 gap-3">
<!-- Card 1: Jan 2025 -->
<div class="bg-surface-container-lowest border border-outline-variant rounded-xl p-4 flex flex-col justify-between hover:shadow-md transition-shadow">
<div>
<div class="flex items-center justify-between mb-2">
<span class="text-label-md font-label-md font-bold text-on-surface">January 2025</span>
<span class="px-2 py-0.5 rounded-full text-label-sm font-label-sm bg-[#CCFBF1] text-[#0F766E] border border-[#99F6E4]">Paid</span>
</div>
<div class="text-data-currency-lg font-data-currency-lg text-on-surface font-bold">£2,140.10</div>
<p class="text-body-sm font-body-sm text-on-surface-variant mt-1">146.5 hours • Barclays •••• 4821</p>
</div>
<div class="mt-4 pt-3 border-t border-surface-container flex items-center justify-between">
<span class="text-label-sm font-label-sm text-on-surface-variant">Paid 31 Jan 2025</span>
<button class="inline-flex items-center gap-1 text-label-md font-label-md text-secondary hover:text-on-secondary-container font-semibold">
<span class="material-symbols-outlined text-[16px]">download</span>
<span>PDF</span>
</button>
</div>
</div>
<!-- Card 2: Dec 2024 -->
<div class="bg-surface-container-lowest border border-outline-variant rounded-xl p-4 flex flex-col justify-between hover:shadow-md transition-shadow">
<div>
<div class="flex items-center justify-between mb-2">
<span class="text-label-md font-label-md font-bold text-on-surface">December 2024</span>
<span class="px-2 py-0.5 rounded-full text-label-sm font-label-sm bg-[#FFE4E6] text-[#9F1239] border border-[#FECDD3]">Holiday Bank</span>
</div>
<div class="text-data-currency-lg font-data-currency-lg text-on-surface font-bold">£2,410.50</div>
<p class="text-body-sm font-body-sm text-on-surface-variant mt-1">162.0 hours (Inc Bank Holiday)</p>
</div>
<div class="mt-4 pt-3 border-t border-surface-container flex items-center justify-between">
<span class="text-label-sm font-label-sm text-on-surface-variant">Paid 24 Dec 2024</span>
<button class="inline-flex items-center gap-1 text-label-md font-label-md text-secondary hover:text-on-secondary-container font-semibold">
<span class="material-symbols-outlined text-[16px]">download</span>
<span>PDF</span>
</button>
</div>
</div>
<!-- Card 3: Nov 2024 -->
<div class="bg-surface-container-lowest border border-outline-variant rounded-xl p-4 flex flex-col justify-between hover:shadow-md transition-shadow">
<div>
<div class="flex items-center justify-between mb-2">
<span class="text-label-md font-label-md font-bold text-on-surface">November 2024</span>
<span class="px-2 py-0.5 rounded-full text-label-sm font-label-sm bg-[#CCFBF1] text-[#0F766E] border border-[#99F6E4]">Paid</span>
</div>
<div class="text-data-currency-lg font-data-currency-lg text-on-surface font-bold">£1,985.40</div>
<p class="text-body-sm font-body-sm text-on-surface-variant mt-1">138.0 hours • Barclays •••• 4821</p>
</div>
<div class="mt-4 pt-3 border-t border-surface-container flex items-center justify-between">
<span class="text-label-sm font-label-sm text-on-surface-variant">Paid 29 Nov 2024</span>
<button class="inline-flex items-center gap-1 text-label-md font-label-md text-secondary hover:text-on-secondary-container font-semibold">
<span class="material-symbols-outlined text-[16px]">download</span>
<span>PDF</span>
</button>
</div>
</div>
</div>
</div>
</main>
<!-- PERSISTENT BOTTOM NAVIGATION (from Shared Components JSON) -->
<!-- Highlight active tab: 'Payslips' matching exact intent -->
<nav class="fixed bottom-0 left-0 w-full z-50 flex justify-around items-center px-margin py-2 pb-safe bg-surface-container-lowest dark:bg-surface-container-low shadow-[0_8px_24px_-4px_rgba(15,31,44,0.08),0_2px_6px_-1px_rgba(15,31,44,0.04)]">
<!-- Item 1: Tracker -->
<a class="flex flex-col items-center justify-center text-on-surface-variant dark:text-surface-variant px-3 py-1.5 hover:text-on-surface dark:hover:text-inverse-on-surface transition-colors active:translate-y-px" href="#">
<span class="material-symbols-outlined text-[22px]">schedule</span>
<span class="text-label-sm font-label-sm mt-0.5">Tracker</span>
</a>
<!-- Item 2: Calculator -->
<a class="flex flex-col items-center justify-center text-on-surface-variant dark:text-surface-variant px-3 py-1.5 hover:text-on-surface dark:hover:text-inverse-on-surface transition-colors active:translate-y-px" href="#">
<span class="material-symbols-outlined text-[22px]">calculate</span>
<span class="text-label-sm font-label-sm mt-0.5">Calculator</span>
</a>
<!-- Item 3: Rota -->
<a class="flex flex-col items-center justify-center text-on-surface-variant dark:text-surface-variant px-3 py-1.5 hover:text-on-surface dark:hover:text-inverse-on-surface transition-colors active:translate-y-px" href="#">
<span class="material-symbols-outlined text-[22px]">calendar_month</span>
<span class="text-label-sm font-label-sm mt-0.5">Rota</span>
</a>
<!-- Item 4: Payslips (ACTIVE Destination) -->
<a class="flex flex-col items-center justify-center bg-secondary-container dark:bg-tertiary-container text-on-secondary-container dark:text-on-tertiary-container rounded-lg px-3 py-1.5 hover:text-on-surface dark:hover:text-inverse-on-surface transition-colors active:translate-y-px" href="#">
<span class="material-symbols-outlined text-[22px]" style="font-variation-settings: 'FILL' 1;">receipt_long</span>
<span class="text-label-sm font-label-sm font-semibold mt-0.5">Payslips</span>
</a>
</nav>
</body></html>
