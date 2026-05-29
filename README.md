<!DOCTYPE html>
<!-- saved from url=(0045)file:///C:/Users/ASUS/Downloads/projexid.html -->
<html lang="ar" dir="rtl"><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">

<meta name="mobile-web-app-capable" content="yes">
<meta name="apple-mobile-web-app-capable" content="yes">
<meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
<meta name="theme-color" content="#1C1C1A">
<meta name="format-detection" content="telephone=no">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ProjexID — نظام إدارة المشاريع الهندسية</title>
<style>

/* System Arabic fonts — fully offline */
:root {
  --font: 'Segoe UI', Tahoma, 'Arial Unicode MS', Arial, sans-serif;
}
body { font-family: var(--font); }


/* ═══ INLINE SVG ICON SYSTEM (replaces tabler icons webfont) ═══ */
.ti {
  display: inline-block;
  width: 1em;
  height: 1em;
  vertical-align: middle;
  background-repeat: no-repeat;
  background-size: contain;
  background-position: center;
}

.ti-alert-triangle { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M12%209v4%22%20%2F%3E%3Cpath%20d%3D%22M10.363%203.591l-8.106%2013.534a1.914%201.914%200%200%200%201.636%202.871h16.214a1.914%201.914%200%200%200%201.636%20-2.871l-8.106%20-13.534a1.914%201.914%200%200%200%20-3.274%200z%22%20%2F%3E%3Cpath%20d%3D%22M12%2016h.01%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-arrow-down { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M12%205l0%2014%22%20%2F%3E%3Cpath%20d%3D%22M18%2013l-6%206%22%20%2F%3E%3Cpath%20d%3D%22M6%2013l6%206%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-arrow-left { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M5%2012l14%200%22%20%2F%3E%3Cpath%20d%3D%22M5%2012l6%206%22%20%2F%3E%3Cpath%20d%3D%22M5%2012l6%20-6%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-arrow-right { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M5%2012l14%200%22%20%2F%3E%3Cpath%20d%3D%22M13%2018l6%20-6%22%20%2F%3E%3Cpath%20d%3D%22M13%206l6%206%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-arrow-up { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M12%205l0%2014%22%20%2F%3E%3Cpath%20d%3D%22M18%2011l-6%20-6%22%20%2F%3E%3Cpath%20d%3D%22M6%2011l6%20-6%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-brand-whatsapp { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M3%2021l1.65%20-3.8a9%209%200%201%201%203.4%202.9l-5.05%20.9%22%20%2F%3E%3Cpath%20d%3D%22M9%2010a.5%20.5%200%200%200%201%200v-1a.5%20.5%200%200%200%20-1%200v1a5%205%200%200%200%205%205h1a.5%20.5%200%200%200%200%20-1h-1a.5%20.5%200%200%200%200%201%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-briefcase { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M3%207m0%202a2%202%200%200%201%202%20-2h14a2%202%200%200%201%202%202v9a2%202%200%200%201%20-2%202h-14a2%202%200%200%201%20-2%20-2z%22%20%2F%3E%3Cpath%20d%3D%22M8%207v-2a2%202%200%200%201%202%20-2h4a2%202%200%200%201%202%202v2%22%20%2F%3E%3Cpath%20d%3D%22M12%2012l0%20.01%22%20%2F%3E%3Cpath%20d%3D%22M3%2013a20%2020%200%200%200%2018%200%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-building { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M3%2021l18%200%22%20%2F%3E%3Cpath%20d%3D%22M9%208l1%200%22%20%2F%3E%3Cpath%20d%3D%22M9%2012l1%200%22%20%2F%3E%3Cpath%20d%3D%22M9%2016l1%200%22%20%2F%3E%3Cpath%20d%3D%22M14%208l1%200%22%20%2F%3E%3Cpath%20d%3D%22M14%2012l1%200%22%20%2F%3E%3Cpath%20d%3D%22M14%2016l1%200%22%20%2F%3E%3Cpath%20d%3D%22M5%2021v-16a2%202%200%200%201%202%20-2h10a2%202%200%200%201%202%202v16%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-building-arch { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M3%2021l18%200%22%20%2F%3E%3Cpath%20d%3D%22M4%2021v-15a2%202%200%200%201%202%20-2h12a2%202%200%200%201%202%202v15%22%20%2F%3E%3Cpath%20d%3D%22M9%2021v-8a3%203%200%200%201%206%200v8%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-building-bank { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M3%2021l18%200%22%20%2F%3E%3Cpath%20d%3D%22M3%2010l18%200%22%20%2F%3E%3Cpath%20d%3D%22M5%2010l0%2011%22%20%2F%3E%3Cpath%20d%3D%22M19%2010l0%2011%22%20%2F%3E%3Cpath%20d%3D%22M9%2010l0%2011%22%20%2F%3E%3Cpath%20d%3D%22M15%2010l0%2011%22%20%2F%3E%3Cpath%20d%3D%22M3%2010l9%20-7l9%207%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-building-warehouse { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M3%2021v-13l9%20-4l9%204v13%22%20%2F%3E%3Cpath%20d%3D%22M13%2013h4v8h-14v-8h4%22%20%2F%3E%3Cpath%20d%3D%22M13%2021v-5a1%201%200%200%200%20-1%20-1h-2a1%201%200%200%200%20-1%201v5%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-calendar { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M4%207a2%202%200%200%201%202%20-2h12a2%202%200%200%201%202%202v12a2%202%200%200%201%20-2%202h-12a2%202%200%200%201%20-2%20-2v-12z%22%20%2F%3E%3Cpath%20d%3D%22M16%203v4%22%20%2F%3E%3Cpath%20d%3D%22M8%203v4%22%20%2F%3E%3Cpath%20d%3D%22M4%2011h16%22%20%2F%3E%3Cpath%20d%3D%22M11%2015h1%22%20%2F%3E%3Cpath%20d%3D%22M12%2015v3%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-camera { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M5%207h1a2%202%200%200%200%202%20-2a1%201%200%200%201%201%20-1h6a1%201%200%200%201%201%201a2%202%200%200%200%202%202h1a2%202%200%200%201%202%202v9a2%202%200%200%201%20-2%202h-14a2%202%200%200%201%20-2%20-2v-9a2%202%200%200%201%202%20-2%22%20%2F%3E%3Cpath%20d%3D%22M9%2013a3%203%200%201%200%206%200a3%203%200%200%200%20-6%200%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-cash { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M7%209m0%202a2%202%200%200%201%202%20-2h10a2%202%200%200%201%202%202v6a2%202%200%200%201%20-2%202h-10a2%202%200%200%201%20-2%20-2z%22%20%2F%3E%3Cpath%20d%3D%22M14%2014m-2%200a2%202%200%201%200%204%200a2%202%200%200%200%20-4%200%22%20%2F%3E%3Cpath%20d%3D%22M17%209v-2a2%202%200%200%200%20-2%20-2h-10a2%202%200%200%200%20-2%202v6a2%202%200%200%200%202%202h2%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-chart-bar { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M3%2012m0%201a1%201%200%200%201%201%20-1h4a1%201%200%200%201%201%201v6a1%201%200%200%201%20-1%201h-4a1%201%200%200%201%20-1%20-1z%22%20%2F%3E%3Cpath%20d%3D%22M9%208m0%201a1%201%200%200%201%201%20-1h4a1%201%200%200%201%201%201v10a1%201%200%200%201%20-1%201h-4a1%201%200%200%201%20-1%20-1z%22%20%2F%3E%3Cpath%20d%3D%22M15%204m0%201a1%201%200%200%201%201%20-1h4a1%201%200%200%201%201%201v14a1%201%200%200%201%20-1%201h-4a1%201%200%200%201%20-1%20-1z%22%20%2F%3E%3Cpath%20d%3D%22M4%2020l14%200%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-check { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M5%2012l5%205l10%20-10%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-checklist { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M9.615%2020h-2.615a2%202%200%200%201%20-2%20-2v-12a2%202%200%200%201%202%20-2h8a2%202%200%200%201%202%202v8%22%20%2F%3E%3Cpath%20d%3D%22M14%2019l2%202l4%20-4%22%20%2F%3E%3Cpath%20d%3D%22M9%208h4%22%20%2F%3E%3Cpath%20d%3D%22M9%2012h2%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-chevron-down { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M6%209l6%206l6%20-6%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-chevron-left { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M15%206l-6%206l6%206%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-clipboard { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M9%205h-2a2%202%200%200%200%20-2%202v12a2%202%200%200%200%202%202h10a2%202%200%200%200%202%20-2v-12a2%202%200%200%200%20-2%20-2h-2%22%20%2F%3E%3Cpath%20d%3D%22M9%203m0%202a2%202%200%200%201%202%20-2h2a2%202%200%200%201%202%202v0a2%202%200%200%201%20-2%202h-2a2%202%200%200%201%20-2%20-2z%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-clipboard-list { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M9%205h-2a2%202%200%200%200%20-2%202v12a2%202%200%200%200%202%202h10a2%202%200%200%200%202%20-2v-12a2%202%200%200%200%20-2%20-2h-2%22%20%2F%3E%3Cpath%20d%3D%22M9%203m0%202a2%202%200%200%201%202%20-2h2a2%202%200%200%201%202%202v0a2%202%200%200%201%20-2%202h-2a2%202%200%200%201%20-2%20-2z%22%20%2F%3E%3Cpath%20d%3D%22M9%2012h6%22%20%2F%3E%3Cpath%20d%3D%22M9%2016h6%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-clock { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M3%2012a9%209%200%201%200%2018%200a9%209%200%200%200%20-18%200%22%20%2F%3E%3Cpath%20d%3D%22M12%207v5l3%203%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-cloud-upload { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M7%2018a4.6%204.4%200%200%201%200%20-9a5%204.5%200%200%201%2011%202h1a3.5%203.5%200%200%201%200%207h-1%22%20%2F%3E%3Cpath%20d%3D%22M9%2015l3%20-3l3%203%22%20%2F%3E%3Cpath%20d%3D%22M12%2012l0%209%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-coin { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M12%2012m-9%200a9%209%200%201%200%2018%200a9%209%200%200%200%20-18%200%22%20%2F%3E%3Cpath%20d%3D%22M14.8%209a2%202%200%200%200%20-1.8%20-1h-2a2%202%200%201%200%200%204h2a2%202%200%201%200%200%204h-2a2%202%200%200%201%20-1.8%20-1%22%20%2F%3E%3Cpath%20d%3D%22M12%207v10%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-dashboard { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M12%2013m-2%200a2%202%200%201%200%204%200a2%202%200%200%200%20-4%200%22%20%2F%3E%3Cpath%20d%3D%22M13.45%2011.55l2.05%20-2.05%22%20%2F%3E%3Cpath%20d%3D%22M6.4%2020a6%206%200%201%201%2011.2%200z%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-database { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M12%206m-8%200a8%203%200%201%200%2016%200a8%203%200%200%200%20-16%200%22%20%2F%3E%3Cpath%20d%3D%22M4%206v6a8%203%200%200%200%2016%200v-6%22%20%2F%3E%3Cpath%20d%3D%22M4%2012v6a8%203%200%200%200%2016%200v-6%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-database-export { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M4%206c0%201.657%203.582%203%208%203s8%20-1.343%208%20-3s-3.582%20-3%20-8%20-3s-8%201.343%20-8%203%22%20%2F%3E%3Cpath%20d%3D%22M4%206v6c0%201.657%203.582%203%208%203c.856%200%201.683%20-.05%202.468%20-.143%22%20%2F%3E%3Cpath%20d%3D%22M20%2012v-6%22%20%2F%3E%3Cpath%20d%3D%22M4%2012v6c0%201.657%203.582%203%208%203c.171%200%20.341%20-.002%20.51%20-.007%22%20%2F%3E%3Cpath%20d%3D%22M16%2019h6%22%20%2F%3E%3Cpath%20d%3D%22M19%2016l3%203l-3%203%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-database-import { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M4%206c0%201.657%203.582%203%208%203s8%20-1.343%208%20-3s-3.582%20-3%20-8%20-3s-8%201.343%20-8%203%22%20%2F%3E%3Cpath%20d%3D%22M4%206v6c0%201.657%203.582%203%208%203c.856%200%201.683%20-.05%202.468%20-.143%22%20%2F%3E%3Cpath%20d%3D%22M20%2012v-6%22%20%2F%3E%3Cpath%20d%3D%22M4%2012v6c0%201.657%203.582%203%208%203c.171%200%20.341%20-.002%20.51%20-.007%22%20%2F%3E%3Cpath%20d%3D%22M19%2016l-3%203l3%203%22%20%2F%3E%3Cpath%20d%3D%22M22%2019h-6%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-device-floppy { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M6%204h10l4%204v10a2%202%200%200%201%20-2%202h-12a2%202%200%200%201%20-2%20-2v-12a2%202%200%200%201%202%20-2%22%20%2F%3E%3Cpath%20d%3D%22M12%2014m-2%200a2%202%200%201%200%204%200a2%202%200%200%200%20-4%200%22%20%2F%3E%3Cpath%20d%3D%22M14%204l0%204l-6%200l0%20-4%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-download { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M4%2017v2a2%202%200%200%200%202%202h12a2%202%200%200%200%202%20-2v-2%22%20%2F%3E%3Cpath%20d%3D%22M7%2011l5%205l5%20-5%22%20%2F%3E%3Cpath%20d%3D%22M12%204l0%2012%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-edit { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M7%207h-1a2%202%200%200%200%20-2%202v9a2%202%200%200%200%202%202h9a2%202%200%200%200%202%20-2v-1%22%20%2F%3E%3Cpath%20d%3D%22M20.385%206.585a2.1%202.1%200%200%200%20-2.97%20-2.97l-8.415%208.385v3h3l8.385%20-8.415z%22%20%2F%3E%3Cpath%20d%3D%22M16%205l3%203%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-external-link { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M12%206h-6a2%202%200%200%200%20-2%202v10a2%202%200%200%200%202%202h10a2%202%200%200%200%202%20-2v-6%22%20%2F%3E%3Cpath%20d%3D%22M11%2013l9%20-9%22%20%2F%3E%3Cpath%20d%3D%22M15%204h5v5%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-eye { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M10%2012a2%202%200%201%200%204%200a2%202%200%200%200%20-4%200%22%20%2F%3E%3Cpath%20d%3D%22M21%2012c-2.4%204%20-5.4%206%20-9%206c-3.6%200%20-6.6%20-2%20-9%20-6c2.4%20-4%205.4%20-6%209%20-6c3.6%200%206.6%202%209%206%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-file { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M14%203v4a1%201%200%200%200%201%201h4%22%20%2F%3E%3Cpath%20d%3D%22M17%2021h-10a2%202%200%200%201%20-2%20-2v-14a2%202%200%200%201%202%20-2h7l5%205v11a2%202%200%200%201%20-2%202z%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-file-description { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M14%203v4a1%201%200%200%200%201%201h4%22%20%2F%3E%3Cpath%20d%3D%22M17%2021h-10a2%202%200%200%201%20-2%20-2v-14a2%202%200%200%201%202%20-2h7l5%205v11a2%202%200%200%201%20-2%202z%22%20%2F%3E%3Cpath%20d%3D%22M9%2017h6%22%20%2F%3E%3Cpath%20d%3D%22M9%2013h6%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-file-invoice { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M14%203v4a1%201%200%200%200%201%201h4%22%20%2F%3E%3Cpath%20d%3D%22M17%2021h-10a2%202%200%200%201%20-2%20-2v-14a2%202%200%200%201%202%20-2h7l5%205v11a2%202%200%200%201%20-2%202z%22%20%2F%3E%3Cpath%20d%3D%22M9%207h4%22%20%2F%3E%3Cpath%20d%3D%22M9%2013h6%22%20%2F%3E%3Cpath%20d%3D%22M13%2017h2%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-file-spreadsheet { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M14%203v4a1%201%200%200%200%201%201h4%22%20%2F%3E%3Cpath%20d%3D%22M17%2021h-10a2%202%200%200%201%20-2%20-2v-14a2%202%200%200%201%202%20-2h7l5%205v11a2%202%200%200%201%20-2%202z%22%20%2F%3E%3Cpath%20d%3D%22M8%2011h8v7h-8z%22%20%2F%3E%3Cpath%20d%3D%22M8%2015h8%22%20%2F%3E%3Cpath%20d%3D%22M11%2011v7%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-file-text { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M14%203v4a1%201%200%200%200%201%201h4%22%20%2F%3E%3Cpath%20d%3D%22M17%2021h-10a2%202%200%200%201%20-2%20-2v-14a2%202%200%200%201%202%20-2h7l5%205v11a2%202%200%200%201%20-2%202z%22%20%2F%3E%3Cpath%20d%3D%22M9%209h1%22%20%2F%3E%3Cpath%20d%3D%22M9%2013h6%22%20%2F%3E%3Cpath%20d%3D%22M9%2017h6%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-files { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M15%203v4a1%201%200%200%200%201%201h4%22%20%2F%3E%3Cpath%20d%3D%22M18%2017h-7a2%202%200%200%201%20-2%20-2v-10a2%202%200%200%201%202%20-2h4l5%205v7a2%202%200%200%201%20-2%202z%22%20%2F%3E%3Cpath%20d%3D%22M16%2017v2a2%202%200%200%201%20-2%202h-7a2%202%200%200%201%20-2%20-2v-11a2%202%200%200%201%202%20-2h2%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-folder { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M5%204h4l3%203h7a2%202%200%200%201%202%202v8a2%202%200%200%201%20-2%202h-14a2%202%200%200%201%20-2%20-2v-11a2%202%200%200%201%202%20-2%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-folder-open { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M5%2019l2.757%20-7.351a1%201%200%200%201%20.936%20-.649h12.307a1%201%200%200%201%20.986%201.164l-.996%205.211a2%202%200%200%201%20-1.964%201.625h-14.026a2%202%200%200%201%20-2%20-2v-11a2%202%200%200%201%202%20-2h4l3%203h7a2%202%200%200%201%202%202v2h-3%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-folders { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M9%204h3l2%202h5a2%202%200%200%201%202%202v7a2%202%200%200%201%20-2%202h-10a2%202%200%200%201%20-2%20-2v-9a2%202%200%200%201%202%20-2%22%20%2F%3E%3Cpath%20d%3D%22M17%2017v2a2%202%200%200%201%20-2%202h-10a2%202%200%200%201%20-2%20-2v-9a2%202%200%200%201%202%20-2h2%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-hard-hat { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M6%2017l-2%204h16l-2%20-4%22%20%2F%3E%3Cpath%20d%3D%22M4%2017h16%22%20%2F%3E%3Cpath%20d%3D%22M12%206v-3%22%20%2F%3E%3Cpath%20d%3D%22M6%2017a6%206%200%200%201%2012%200%22%20%2F%3E%3Cpath%20d%3D%22M12%203a9%209%200%200%201%209%209h-1%22%20%2F%3E%3Cpath%20d%3D%22M3%2012h-1a9%209%200%200%201%209%20-9%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-hash { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M5%209l14%200%22%20%2F%3E%3Cpath%20d%3D%22M5%2015l14%200%22%20%2F%3E%3Cpath%20d%3D%22M11%204l-4%2016%22%20%2F%3E%3Cpath%20d%3D%22M17%204l-4%2016%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-history { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M12%208l0%204l2%202%22%20%2F%3E%3Cpath%20d%3D%22M3.05%2011a9%209%200%201%201%20.5%204m-.5%205v-5h5%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-info-circle { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M3%2012a9%209%200%201%200%2018%200a9%209%200%200%200%20-18%200%22%20%2F%3E%3Cpath%20d%3D%22M12%209h.01%22%20%2F%3E%3Cpath%20d%3D%22M11%2012h1v4h1%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-key { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M16.555%203.843l3.602%203.602a2.877%202.877%200%200%201%200%204.069l-2.643%202.643a2.877%202.877%200%200%201%20-4.069%200l-.301%20-.301l-6.558%206.558a2%202%200%200%201%20-1.239%20.578l-.175%20.008h-1.172a1%201%200%200%201%20-.993%20-.883l-.007%20-.117v-1.172a2%202%200%200%201%20.467%20-1.284l.119%20-.13l.414%20-.414h2v-2h2v-2l2.144%20-2.144l-.301%20-.301a2.877%202.877%200%200%201%200%20-4.069l2.643%20-2.643a2.877%202.877%200%200%201%204.069%200z%22%20%2F%3E%3Cpath%20d%3D%22M15%209h.01%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-layout-columns { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M4%206a2%202%200%200%201%202%20-2h3a2%202%200%200%201%202%202v12a2%202%200%200%201%20-2%202h-3a2%202%200%200%201%20-2%20-2v-12z%22%20%2F%3E%3Cpath%20d%3D%22M13%206a2%202%200%200%201%202%20-2h3a2%202%200%200%201%202%202v12a2%202%200%200%201%20-2%202h-3a2%202%200%200%201%20-2%20-2v-12z%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-layout-kanban { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M4%204m0%202a2%202%200%200%201%202%20-2h2a2%202%200%200%201%202%202v14a2%202%200%200%201%20-2%202h-2a2%202%200%200%201%20-2%20-2z%22%20%2F%3E%3Cpath%20d%3D%22M14%204m0%202a2%202%200%200%201%202%20-2h2a2%202%200%200%201%202%202v8a2%202%200%200%201%20-2%202h-2a2%202%200%200%201%20-2%20-2z%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-layout-list { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M4%204m0%202a2%202%200%200%201%202%20-2h2a2%202%200%200%201%202%202v2a2%202%200%200%201%20-2%202h-2a2%202%200%200%201%20-2%20-2z%22%20%2F%3E%3Cpath%20d%3D%22M4%2014m0%202a2%202%200%200%201%202%20-2h2a2%202%200%200%201%202%202v2a2%202%200%200%201%20-2%202h-2a2%202%200%200%201%20-2%20-2z%22%20%2F%3E%3Cpath%20d%3D%22M14%206l6%200%22%20%2F%3E%3Cpath%20d%3D%22M14%2010l6%200%22%20%2F%3E%3Cpath%20d%3D%22M14%2016l6%200%22%20%2F%3E%3Cpath%20d%3D%22M14%2020l6%200%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-list { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M9%206l11%200%22%20%2F%3E%3Cpath%20d%3D%22M9%2012l11%200%22%20%2F%3E%3Cpath%20d%3D%22M9%2018l11%200%22%20%2F%3E%3Cpath%20d%3D%22M5%206l0%20.01%22%20%2F%3E%3Cpath%20d%3D%22M5%2012l0%20.01%22%20%2F%3E%3Cpath%20d%3D%22M5%2018l0%20.01%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-list-check { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M3.5%205.5l1.5%201.5l2.5%20-2.5%22%20%2F%3E%3Cpath%20d%3D%22M3.5%2011.5l1.5%201.5l2.5%20-2.5%22%20%2F%3E%3Cpath%20d%3D%22M3.5%2017.5l1.5%201.5l2.5%20-2.5%22%20%2F%3E%3Cpath%20d%3D%22M11%206l9%200%22%20%2F%3E%3Cpath%20d%3D%22M11%2012l9%200%22%20%2F%3E%3Cpath%20d%3D%22M11%2018l9%200%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-list-numbers { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M11%206h9%22%20%2F%3E%3Cpath%20d%3D%22M11%2012h9%22%20%2F%3E%3Cpath%20d%3D%22M12%2018h8%22%20%2F%3E%3Cpath%20d%3D%22M4%2016a2%202%200%201%201%204%200c0%20.591%20-.5%201%20-1%201.5l-3%202.5h4%22%20%2F%3E%3Cpath%20d%3D%22M6%2010v-6l-2%202%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-lock { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M5%2013a2%202%200%200%201%202%20-2h10a2%202%200%200%201%202%202v6a2%202%200%200%201%20-2%202h-10a2%202%200%200%201%20-2%20-2v-6z%22%20%2F%3E%3Cpath%20d%3D%22M11%2016a1%201%200%201%200%202%200a1%201%200%200%200%20-2%200%22%20%2F%3E%3Cpath%20d%3D%22M8%2011v-4a4%204%200%201%201%208%200v4%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-logout { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M14%208v-2a2%202%200%200%200%20-2%20-2h-7a2%202%200%200%200%20-2%202v12a2%202%200%200%200%202%202h7a2%202%200%200%200%202%20-2v-2%22%20%2F%3E%3Cpath%20d%3D%22M9%2012h12l-3%20-3%22%20%2F%3E%3Cpath%20d%3D%22M18%2015l3%20-3%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-mail { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M3%207a2%202%200%200%201%202%20-2h14a2%202%200%200%201%202%202v10a2%202%200%200%201%20-2%202h-14a2%202%200%200%201%20-2%20-2v-10z%22%20%2F%3E%3Cpath%20d%3D%22M3%207l9%206l9%20-6%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-map-pin { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M9%2011a3%203%200%201%200%206%200a3%203%200%200%200%20-6%200%22%20%2F%3E%3Cpath%20d%3D%22M17.657%2016.657l-4.243%204.243a2%202%200%200%201%20-2.827%200l-4.244%20-4.243a8%208%200%201%201%2011.314%200z%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-menu-2 { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M4%206l16%200%22%20%2F%3E%3Cpath%20d%3D%22M4%2012l16%200%22%20%2F%3E%3Cpath%20d%3D%22M4%2018l16%200%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-message-circle { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M3%2020l1.3%20-3.9c-2.324%20-3.437%20-1.426%20-7.872%202.1%20-10.374c3.526%20-2.501%208.59%20-2.296%2011.845%20.48c3.255%202.777%203.695%207.266%201.029%2010.501c-2.666%203.235%20-7.615%204.215%20-11.574%202.293l-4.7%201%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-minus { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M5%2012l14%200%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-notes { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M5%203m0%202a2%202%200%200%201%202%20-2h10a2%202%200%200%201%202%202v14a2%202%200%200%201%20-2%202h-10a2%202%200%200%201%20-2%20-2z%22%20%2F%3E%3Cpath%20d%3D%22M9%207l6%200%22%20%2F%3E%3Cpath%20d%3D%22M9%2011l6%200%22%20%2F%3E%3Cpath%20d%3D%22M9%2015l4%200%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-paperclip { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M15%207l-6.5%206.5a1.5%201.5%200%200%200%203%203l6.5%20-6.5a3%203%200%200%200%20-6%20-6l-6.5%206.5a4.5%204.5%200%200%200%209%209l6.5%20-6.5%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-pencil { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M4%2020h4l10.5%20-10.5a2.828%202.828%200%201%200%20-4%20-4l-10.5%2010.5v4%22%20%2F%3E%3Cpath%20d%3D%22M13.5%206.5l4%204%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-phone { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M5%204h4l2%205l-2.5%201.5a11%2011%200%200%200%205%205l1.5%20-2.5l5%202v4a2%202%200%200%201%20-2%202a16%2016%200%200%201%20-15%20-15a2%202%200%200%201%202%20-2%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-photo { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M15%208h.01%22%20%2F%3E%3Cpath%20d%3D%22M3%206a3%203%200%200%201%203%20-3h12a3%203%200%200%201%203%203v12a3%203%200%200%201%20-3%203h-12a3%203%200%200%201%20-3%20-3v-12z%22%20%2F%3E%3Cpath%20d%3D%22M3%2016l5%20-5c.928%20-.893%202.072%20-.893%203%200l5%205%22%20%2F%3E%3Cpath%20d%3D%22M14%2014l1%20-1c.928%20-.893%202.072%20-.893%203%200l3%203%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-plus { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M12%205l0%2014%22%20%2F%3E%3Cpath%20d%3D%22M5%2012l14%200%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-printer { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M17%2017h2a2%202%200%200%200%202%20-2v-4a2%202%200%200%200%20-2%20-2h-14a2%202%200%200%200%20-2%202v4a2%202%200%200%200%202%202h2%22%20%2F%3E%3Cpath%20d%3D%22M17%209v-4a2%202%200%200%200%20-2%20-2h-6a2%202%200%200%200%20-2%202v4%22%20%2F%3E%3Cpath%20d%3D%22M7%2013m0%202a2%202%200%200%201%202%20-2h6a2%202%200%200%201%202%202v4a2%202%200%200%201%20-2%202h-6a2%202%200%200%201%20-2%20-2z%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-receipt { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M5%2021v-16a1%201%200%200%201%201%20-1h12a1%201%200%200%201%201%201v16l-3%20-2l-2%202l-2%20-2l-2%202l-2%20-2l-3%202%22%20%2F%3E%3Cpath%20d%3D%22M14%208h-2.5a1.5%201.5%200%200%200%200%203h1a1.5%201.5%200%200%201%200%203h-2.5m2%200v1.5m0%20-9v1.5%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-receipt-off { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M3%203l18%2018%22%20%2F%3E%3Cpath%20d%3D%22M9%205h9a1%201%200%200%201%201%201v13%22%20%2F%3E%3Cpath%20d%3D%22M19%2019l-3%20-2l-2%202l-2%20-2l-2%202l-2%20-2l-3%202v-14%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-report { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M8%205h-2a2%202%200%200%200%20-2%202v12a2%202%200%200%200%202%202h5.697%22%20%2F%3E%3Cpath%20d%3D%22M18%2014v4h4%22%20%2F%3E%3Cpath%20d%3D%22M18%2011v-4a2%202%200%200%200%20-2%20-2h-2%22%20%2F%3E%3Cpath%20d%3D%22M10%203m0%202a2%202%200%200%201%202%20-2h2a2%202%200%200%201%202%202v0a2%202%200%200%201%20-2%202h-2a2%202%200%200%201%20-2%20-2z%22%20%2F%3E%3Cpath%20d%3D%22M18%2018m-4%200a4%204%200%201%200%208%200a4%204%200%200%200%20-8%200%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-report-analytics { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M9%205h-2a2%202%200%200%200%20-2%202v12a2%202%200%200%200%202%202h10a2%202%200%200%200%202%20-2v-12a2%202%200%200%200%20-2%20-2h-2%22%20%2F%3E%3Cpath%20d%3D%22M9%203m0%202a2%202%200%200%201%202%20-2h2a2%202%200%200%201%202%202v0a2%202%200%200%201%20-2%202h-2a2%202%200%200%201%20-2%20-2z%22%20%2F%3E%3Cpath%20d%3D%22M9%2017v-5%22%20%2F%3E%3Cpath%20d%3D%22M12%2017v-1%22%20%2F%3E%3Cpath%20d%3D%22M15%2017v-3%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-report-off { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M3%203l18%2018%22%20%2F%3E%3Cpath%20d%3D%22M9%205h-2a2%202%200%200%200%20-2%202v12a2%202%200%200%200%202%202h10c.27%200%20.528%20-.033%20.774%20-.096%22%20%2F%3E%3Cpath%20d%3D%22M18.138%2018.138a2%202%200%200%201%20-.138%20.862v-8%22%20%2F%3E%3Cpath%20d%3D%22M10%203m0%202a2%202%200%200%201%202%20-2h2a2%202%200%200%201%202%202v0a2%202%200%200%201%20-2%202h-2a2%202%200%200%201%20-2%20-2z%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-search { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M10%2010m-7%200a7%207%200%201%200%2014%200a7%207%200%200%200%20-14%200%22%20%2F%3E%3Cpath%20d%3D%22M21%2021l-6%20-6%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-send { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M10%2014l11%20-11%22%20%2F%3E%3Cpath%20d%3D%22M21%203l-6.5%2018a.55%20.55%200%200%201%20-1%200l-3.5%20-7l-7%20-3.5a.55%20.55%200%200%201%200%20-1l18%20-6.5%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-settings { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M10.325%204.317c.426%20-1.756%202.924%20-1.756%203.35%200a1.724%201.724%200%200%200%202.573%201.066c1.543%20-.94%203.31%20.826%202.37%202.37a1.724%201.724%200%200%200%201.065%202.572c1.756%20.426%201.756%202.924%200%203.35a1.724%201.724%200%200%200%20-1.066%202.573c.94%201.543%20-.826%203.31%20-2.37%202.37a1.724%201.724%200%200%200%20-2.572%201.065c-.426%201.756%20-2.924%201.756%20-3.35%200a1.724%201.724%200%200%200%20-2.573%20-1.066c-1.543%20.94%20-3.31%20-.826%20-2.37%20-2.37a1.724%201.724%200%200%200%20-1.065%20-2.572c-1.756%20-.426%20-1.756%20-2.924%200%20-3.35a1.724%201.724%200%200%200%201.066%20-2.573c-.94%20-1.543%20.826%20-3.31%202.37%20-2.37c1%20.608%202.296%20.07%202.572%20-1.065z%22%20%2F%3E%3Cpath%20d%3D%22M9%2012a3%203%200%201%200%206%200a3%203%200%200%200%20-6%200%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-settings-cog { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M12.003%2021c-.732%20.001%20-1.465%20-.438%20-1.678%20-1.317a1.724%201.724%200%200%200%20-2.573%20-1.066c-1.543%20.94%20-3.31%20-.826%20-2.37%20-2.37a1.724%201.724%200%200%200%20-1.065%20-2.572c-1.756%20-.426%20-1.756%20-2.924%200%20-3.35a1.724%201.724%200%200%200%201.066%20-2.573c-.94%20-1.543%20.826%20-3.31%202.37%20-2.37c1%20.608%202.296%20.07%202.572%20-1.065c.426%20-1.756%202.924%20-1.756%203.35%200a1.724%201.724%200%200%200%202.573%201.066c1.543%20-.94%203.31%20.826%202.37%202.37a1.724%201.724%200%200%200%20-1.065%202.572%22%20%2F%3E%3Cpath%20d%3D%22M9%2012a3%203%200%201%200%205.252%20-1.997%22%20%2F%3E%3Cpath%20d%3D%22M18%2018m-3%200a3%203%200%201%200%206%200a3%203%200%200%200%20-6%200%22%20%2F%3E%3Cpath%20d%3D%22M21%2021l-1.5%20-1.5%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-shield { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M12%203a12%2012%200%200%200%208.5%203a12%2012%200%200%201%20-8.5%2015a12%2012%200%200%201%20-8.5%20-15a12%2012%200%200%200%208.5%20-3%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-shield-check { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M11.46%2020.846a12%2012%200%200%201%20-7.96%20-14.846a12%2012%200%200%200%208.5%20-3a12%2012%200%200%200%208.5%203a12%2012%200%200%201%20-.09%207.06%22%20%2F%3E%3Cpath%20d%3D%22M15%2019l2%202l4%20-4%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-trash { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M4%207l16%200%22%20%2F%3E%3Cpath%20d%3D%22M10%2011l0%206%22%20%2F%3E%3Cpath%20d%3D%22M14%2011l0%206%22%20%2F%3E%3Cpath%20d%3D%22M5%207l1%2012a2%202%200%200%200%202%202h8a2%202%200%200%200%202%20-2l1%20-12%22%20%2F%3E%3Cpath%20d%3D%22M9%207v-3a1%201%200%200%201%201%20-1h4a1%201%200%200%201%201%201v3%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-upload { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M4%2017v2a2%202%200%200%200%202%202h12a2%202%200%200%200%202%20-2v-2%22%20%2F%3E%3Cpath%20d%3D%22M7%209l5%20-5l5%205%22%20%2F%3E%3Cpath%20d%3D%22M12%204l0%2012%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-user { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M8%207a4%204%200%201%200%208%200a4%204%200%200%200%20-8%200%22%20%2F%3E%3Cpath%20d%3D%22M6%2021v-2a4%204%200%200%201%204%20-4h4a4%204%200%200%201%204%204v2%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-user-edit { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M8%207a4%204%200%201%200%208%200a4%204%200%200%200%20-8%200%22%20%2F%3E%3Cpath%20d%3D%22M6%2021v-2a4%204%200%200%201%204%20-4h2.5%22%20%2F%3E%3Cpath%20d%3D%22M18.42%2015.61a2.1%202.1%200%200%201%202.97%202.97l-3.39%203.42h-3v-3l3.42%20-3.39z%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-user-plus { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M8%207a4%204%200%201%200%208%200a4%204%200%200%200%20-8%200%22%20%2F%3E%3Cpath%20d%3D%22M16%2019h6%22%20%2F%3E%3Cpath%20d%3D%22M19%2016v6%22%20%2F%3E%3Cpath%20d%3D%22M6%2021v-2a4%204%200%200%201%204%20-4h4%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-users { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M9%207m-4%200a4%204%200%201%200%208%200a4%204%200%200%200%20-8%200%22%20%2F%3E%3Cpath%20d%3D%22M3%2021v-2a4%204%200%200%201%204%20-4h4a4%204%200%200%201%204%204v2%22%20%2F%3E%3Cpath%20d%3D%22M16%203.13a4%204%200%200%201%200%207.75%22%20%2F%3E%3Cpath%20d%3D%22M21%2021v-2a4%204%200%200%200%20-3%20-3.85%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-users-group { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M10%2013a2%202%200%201%200%204%200a2%202%200%200%200%20-4%200%22%20%2F%3E%3Cpath%20d%3D%22M8%2021v-1a2%202%200%200%201%202%20-2h4a2%202%200%200%201%202%202v1%22%20%2F%3E%3Cpath%20d%3D%22M15%205a2%202%200%201%200%204%200a2%202%200%200%200%20-4%200%22%20%2F%3E%3Cpath%20d%3D%22M17%2010h2a2%202%200%200%201%202%202v1%22%20%2F%3E%3Cpath%20d%3D%22M5%205a2%202%200%201%200%204%200a2%202%200%200%200%20-4%200%22%20%2F%3E%3Cpath%20d%3D%22M3%2013v-1a2%202%200%200%201%202%20-2h2%22%20%2F%3E%3C%2Fsvg%3E"); }
.ti-x { background-image: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%20fill%3D%22none%22%20stroke%3D%22currentColor%22%20stroke-width%3D%222%22%20stroke-linecap%3D%22round%22%20stroke-linejoin%3D%22round%22%3E%3Cpath%20stroke%3D%22none%22%20d%3D%22M0%200h24v24H0z%22%20fill%3D%22none%22%2F%3E%3Cpath%20d%3D%22M18%206l-12%2012%22%20%2F%3E%3Cpath%20d%3D%22M6%206l12%2012%22%20%2F%3E%3C%2Fsvg%3E"); }

:root {
  --bg: #F2F1EE;
  --surface: #FFFFFF;
  --surface2: #F7F6F3;
  --surface3: #EEEDEA;
  --border: rgba(0,0,0,0.10);
  --border2: rgba(0,0,0,0.18);
  --text1: #1C1C1A;
  --text2: #52524E;
  --text3: #9A9A94;
  --accent: #534AB7;
  --accent-d: #3A338A;
  --accent-light: #EEEDFE;
  --accent-mid: #AFA9EC;
  --client-c: #1E6FA8;
  --client-light: #E3F0FA;
  --project-c: #1A8A5A;
  --project-light: #E1F5EC;
  --exec-c: #B85C1A;
  --exec-light: #FAEEE0;
  --green: #1D9E75;
  --green-light: #E1F5EE;
  --red: #E24B4A;
  --red-light: #FCEBEB;
  --amber: #EF9F27;
  --amber-light: #FAEEDA;
  --blue: #2B7FCC;
  --blue-light: #E3F0FA;
  --radius: 12px;
  --radius-sm: 8px;
  --radius-xs: 5px;
  --shadow: 0 1px 3px rgba(0,0,0,0.07), 0 1px 12px rgba(0,0,0,0.04);
  --shadow-md: 0 4px 16px rgba(0,0,0,0.10), 0 1px 4px rgba(0,0,0,0.06);
  --sidebar-w: 240px;
  --font: 'IBM Plex Sans Arabic', 'Segoe UI', Tahoma, Arial, sans-serif;
}

* { box-sizing: border-box; margin: 0; padding: 0; }
html, body { height: 100%; }
body { font-family: var(--font); background: var(--bg); color: var(--text1); direction: rtl; font-size: 14px; }

/* ═══ LOGIN ═══════════════════════════════════════════════════════ */
.login-wrap {
  position: fixed; inset: 0; z-index: 1200;
  background: linear-gradient(140deg, #1C1A3A 0%, #2D2870 50%, #534AB7 100%);
  display: flex; align-items: center; justify-content: center;
}
.login-card {
  background: rgba(255,255,255,0.97);
  border-radius: 16px; padding: 44px 40px;
  width: 400px; max-width: 95vw;
  box-shadow: 0 24px 80px rgba(0,0,0,0.35);
}
.login-brand { display: flex; align-items: center; gap: 12px; margin-bottom: 32px; }
.login-mark { width: 48px; height: 48px; background: var(--accent); border-radius: 13px; display: flex; align-items: center; justify-content: center; }
.login-mark i { color: #fff; font-size: 26px; }
.login-name { font-size: 22px; font-weight: 700; color: var(--accent); letter-spacing: -0.5px; }
.login-tagline { font-size: 12px; color: var(--text3); margin-top: 1px; }
.login-fields { display: flex; flex-direction: column; gap: 14px; }
.field-wrap { position: relative; }
.field-wrap i { position: absolute; right: 12px; top: 50%; transform: translateY(-50%); color: var(--text3); font-size: 17px; pointer-events: none; }
.lin { width: 100%; padding: 11px 40px 11px 14px; border: 1.5px solid var(--border2); border-radius: var(--radius-sm); font-size: 14px; font-family: var(--font); color: var(--text1); outline: none; transition: border-color 0.15s; }
.lin:focus { border-color: var(--accent); }
.lbtn { width: 100%; padding: 12px; margin-top: 6px; background: var(--accent); color: #fff; border: none; border-radius: var(--radius-sm); font-size: 14px; font-weight: 600; font-family: var(--font); cursor: pointer; transition: background 0.15s; }
.lbtn:hover { background: var(--accent-d); }
.l-hint { margin-top: 20px; padding: 14px; background: var(--bg); border-radius: var(--radius-sm); font-size: 11px; color: var(--text3); line-height: 1.8; }
.l-err { font-size: 12px; color: var(--red); text-align: center; min-height: 16px; }

/* ═══ LAYOUT ══════════════════════════════════════════════════════ */
.app { display: flex; height: 100vh; overflow: hidden; }
.sidebar { width: var(--sidebar-w); background: var(--text1); display: flex; flex-direction: column; flex-shrink: 0; overflow-y: auto; }
.main { flex: 1; display: flex; flex-direction: column; overflow: hidden; min-width: 0; }

/* ═══ SIDEBAR ═════════════════════════════════════════════════════ */
.sb-brand { padding: 20px 18px 16px; display: flex; align-items: center; gap: 11px; border-bottom: 1px solid rgba(255,255,255,0.08); }
.sb-mark { width: 38px; height: 38px; background: var(--accent); border-radius: 10px; display: flex; align-items: center; justify-content: center; flex-shrink: 0; }
.sb-mark i { color: #fff; font-size: 22px; }
.sb-name { font-size: 16px; font-weight: 700; color: #fff; letter-spacing: -0.3px; }
.sb-tag { font-size: 10px; color: rgba(255,255,255,0.4); }

.sb-nav { flex: 1; padding: 10px 0; }
.sb-sec { padding: 14px 18px 5px; font-size: 9.5px; letter-spacing: 1px; text-transform: uppercase; color: rgba(255,255,255,0.3); font-weight: 600; }
.ni { display: flex; align-items: center; gap: 10px; padding: 9px 18px; cursor: pointer; font-size: 13px; color: rgba(255,255,255,0.6); transition: all 0.12s; position: relative; }
.ni:hover { color: rgba(255,255,255,0.9); background: rgba(255,255,255,0.06); }
.ni.on { color: #fff; background: rgba(255,255,255,0.1); }
.ni.on::before { content: ''; position: absolute; right: 0; top: 6px; bottom: 6px; width: 3px; background: var(--accent-mid); border-radius: 3px 0 0 3px; }
.ni i { font-size: 18px; width: 22px; flex-shrink: 0; }
.nbadge { margin-right: auto; background: var(--accent); color: #fff; font-size: 9.5px; padding: 2px 7px; border-radius: 10px; font-weight: 700; }

.sb-user { padding: 14px 18px; border-top: 1px solid rgba(255,255,255,0.08); display: flex; align-items: center; gap: 10px; }
.av { border-radius: 50%; display: flex; align-items: center; justify-content: center; font-weight: 700; color: #fff; flex-shrink: 0; font-size: 11px; }

/* ═══ TOPBAR ══════════════════════════════════════════════════════ */
.topbar { background: var(--surface); border-bottom: 1px solid var(--border); padding: 12px 24px; display: flex; align-items: center; gap: 12px; flex-shrink: 0; }
.pg-title { font-size: 15px; font-weight: 700; color: var(--text1); flex: 1; letter-spacing: -0.2px; }
.tbtn { display: flex; align-items: center; gap: 6px; padding: 8px 14px; border-radius: var(--radius-sm); border: 1px solid var(--border2); background: var(--surface); font-size: 13px; color: var(--text2); cursor: pointer; font-family: var(--font); transition: all 0.12s; white-space: nowrap; }
.tbtn:hover { background: var(--surface2); }
.tbtn.pr { background: var(--accent); color: #fff; border-color: var(--accent); font-weight: 600; }
.tbtn.pr:hover { background: var(--accent-d); border-color: var(--accent-d); }
.tbtn i { font-size: 16px; }
.search-wrap { position: relative; }
.search-wrap i { position: absolute; right: 10px; top: 50%; transform: translateY(-50%); color: var(--text3); font-size: 16px; pointer-events: none; }
.gsearch { padding: 8px 36px 8px 12px; border: 1px solid var(--border); border-radius: var(--radius-sm); font-size: 13px; font-family: var(--font); color: var(--text1); background: var(--surface2); width: 240px; outline: none; transition: all 0.15s; }
.gsearch:focus { border-color: var(--accent); background: var(--surface); width: 280px; }

/* ═══ CONTENT ═════════════════════════════════════════════════════ */
.content { flex: 1; overflow-y: auto; padding: 24px; }
.view { display: none; }
.view.on { display: block; }

/* ═══ STATS ROW ═══════════════════════════════════════════════════ */
.stats-row { display: grid; grid-template-columns: repeat(4,1fr); gap: 14px; margin-bottom: 24px; }
.stat-card { background: var(--surface); border: 1px solid var(--border); border-radius: var(--radius); padding: 18px 20px; box-shadow: var(--shadow); position: relative; overflow: hidden; }
.stat-card::before { content: ''; position: absolute; top: 0; right: 0; width: 4px; height: 100%; }
.stat-card.sc-blue::before { background: var(--blue); }
.stat-card.sc-green::before { background: var(--green); }
.stat-card.sc-amber::before { background: var(--amber); }
.stat-card.sc-red::before { background: var(--red); }
.stat-icon {
  width:100%; border-radius:10px 10px 6px 6px;
  display:flex; align-items:center; gap:10px;
  padding:10px 14px; margin-bottom:14px;
}
.stat-icon i { font-size:26px; flex-shrink:0; }
.stat-icon-label { font-size:15px; font-weight:800; line-height:1.2; flex:1; }
.stat-icon i { font-size: 20px; }
.stat-val { font-size: 28px; font-weight: 700; color: var(--text1); line-height: 1; margin-bottom: 4px; }
.stat-lbl { font-size: 12px; color: var(--text3); }
.stat-sub { font-size: 11px; margin-top: 6px; font-weight: 500; }

/* ═══ SECTION HEADER ══════════════════════════════════════════════ */
.sec-hd { font-size: 13px; font-weight: 700; color: var(--text1); margin-bottom: 14px; display: flex; align-items: center; justify-content: space-between; letter-spacing: -0.1px; }
.sec-hd-link { font-size: 12px; font-weight: 500; color: var(--accent); cursor: pointer; }
.sec-hd-link:hover { text-decoration: underline; }

/* ═══ CARDS / TABLE ═══════════════════════════════════════════════ */
.card { background: var(--surface); border: 1px solid var(--border); border-radius: var(--radius); box-shadow: var(--shadow); }
.tbl-wrap { overflow-x: auto; }
table { width: 100%; border-collapse: collapse; }
th { font-size: 11px; font-weight: 600; color: var(--text3); padding: 10px 14px; text-align: right; border-bottom: 1px solid var(--border); letter-spacing: 0.3px; text-transform: uppercase; background: var(--surface2); }
th:first-child { border-radius: 0 var(--radius-sm) 0 0; }
th:last-child { border-radius: var(--radius-sm) 0 0 0; }
td { padding: 12px 14px; border-bottom: 1px solid var(--border); font-size: 13px; color: var(--text1); vertical-align: middle; }
tr:last-child td { border-bottom: none; }
tr:hover td { background: var(--surface2); }

/* ═══ BADGES ══════════════════════════════════════════════════════ */
.badge { display: inline-flex; align-items: center; gap: 4px; padding: 3px 9px; border-radius: 20px; font-size: 11px; font-weight: 600; white-space: nowrap; }
.badge-urgent { background: #FAECE7; color: #7A2F12; }
.badge-medium { background: var(--amber-light); color: #6B3D07; }
.badge-low { background: #EAF3DE; color: #2D5409; }
.badge-waiting { background: var(--surface3); color: var(--text2); }
.badge-inprog { background: var(--blue-light); color: #1040A0; }
.badge-review { background: var(--amber-light); color: #7A5000; }
.badge-done { background: var(--green-light); color: #0a5c3f; }
.badge-hold { background: #F3E8FD; color: #5A1A7A; }
.badge-waitclient { background: #FCF0DB; color: #7A4500; }
.badge-design { background: #FFEAE8; color: #B03030; }
.badge-permit { background: #E3F5FD; color: #1060A0; }
.badge-super { background: #FFFCE0; color: #7A7000; }
.badge-exec { background: #E8F7F0; color: #1A7050; }
.badge-admin { background: #EEE8FD; color: #5030A0; }
.badge-paid { background: var(--green-light); color: #0a5c3f; }
.badge-unpaid { background: var(--red-light); color: #8b2020; }
.badge-partial { background: var(--amber-light); color: #6B3D07; }

/* ═══ PROGRESS BAR ════════════════════════════════════════════════ */
.prog-bar { height: 6px; background: var(--surface3); border-radius: 3px; overflow: hidden; min-width: 80px; }
.prog-fill { height: 100%; border-radius: 3px; background: linear-gradient(90deg, var(--accent), var(--accent-mid)); transition: width 0.3s; }

.dash-type-grid { display: grid; grid-template-columns: repeat(5, minmax(0, 1fr)); gap: 14px; }
.dash-type-column { background: var(--surface); border: 1px solid var(--border); border-radius: 16px; padding: 14px; display: flex; flex-direction: column; min-height: 220px; }
.dash-type-column.clickable { cursor: pointer; transition: transform 0.15s ease, border-color 0.15s ease, box-shadow 0.15s ease; }
.dash-type-column.clickable:hover { transform: translateY(-1px); border-color: var(--accent); box-shadow: 0 10px 30px rgba(0,0,0,0.06); }
.dash-type-header { display: flex; align-items: center; gap: 10px; font-size: 13px; font-weight: 700; color: var(--text1); }
.dash-type-icon { width: 26px; height: 26px; display: inline-flex; align-items: center; justify-content: center; border-radius: 50%; background: var(--surface2); font-size: 16px; }
.dash-type-label { color: var(--text1); }
.dash-type-list { margin: 12px 0 10px; display: flex; flex-direction: column; gap: 8px; overflow-y: auto; max-height: 220px; }
.dash-type-item { font-size: 12px; color: var(--text2); padding: 8px 10px; background: var(--surface2); border-radius: 10px; }
.dash-type-empty { font-size: 12px; color: var(--text3); text-align: center; padding: 16px 0; }
.dash-type-summary { display: grid; grid-template-columns: 1fr; gap: 6px; border-top: 1px solid var(--border); padding-top: 10px; font-size: 12px; color: var(--text2); }
.dash-type-summary div { display: flex; justify-content: space-between; align-items: center; gap: 10px; }
.dash-type-summary strong { color: var(--text1); }
.dash-summary-grid { display: grid; grid-template-columns: repeat(6, minmax(0, 1fr)); gap: 10px; margin-top: 18px; }
.dash-summary-card { background: var(--surface2); border: 1px solid var(--border); border-radius: 14px; padding: 14px; display: flex; flex-direction: column; gap: 6px; }
.dash-summary-label { font-size: 12px; color: var(--text3); line-height: 1.3; display: flex; flex-direction: column; gap: 2px; }
.dash-summary-label span:first-child { font-weight: 700; color: var(--text1); }
.dash-summary-val { font-size: 18px; font-weight: 700; color: var(--text1); }
@media (max-width: 1100px) { .dash-summary-grid { grid-template-columns: repeat(3, minmax(0, 1fr)); } }
@media (max-width: 720px) { .dash-summary-grid { grid-template-columns: repeat(2, minmax(0, 1fr)); } }

/* ═══ ICON BUTTONS ════════════════════════════════════════════════ */
.icon-btn { width: 32px; height: 32px; border-radius: var(--radius-sm); border: 1px solid var(--border); background: var(--surface); display: inline-flex; align-items: center; justify-content: center; cursor: pointer; color: var(--text3); transition: all 0.12s; font-family: var(--font); }
.icon-btn:hover { background: var(--surface2); color: var(--text1); border-color: var(--border2); }
.icon-btn.del:hover { background: var(--red-light); color: #8b2020; border-color: #f09595; }
.icon-btn.edit:hover { background: var(--accent-light); color: var(--accent); border-color: var(--accent-mid); }
.icon-btn i { font-size: 15px; }
.act-row { display: flex; gap: 5px; }

/* ═══ FILTER BAR ══════════════════════════════════════════════════ */
.filter-bar { display: flex; align-items: center; gap: 10px; margin-bottom: 16px; flex-wrap: wrap; }
.finput, .fselect { padding: 8px 12px; border: 1px solid var(--border); border-radius: var(--radius-sm); font-size: 13px; color: var(--text1); background: var(--surface); font-family: var(--font); outline: none; box-shadow: var(--shadow); }
.finput { min-width: 200px; }
.finput:focus, .fselect:focus { border-color: var(--accent); }

/* ═══ MODALS ══════════════════════════════════════════════════════ */
.overlay { position: fixed; inset: 0; background: rgba(0,0,0,0.5); z-index: 900; display: none; align-items: flex-start; justify-content: center; overflow-y: auto; padding: 30px 16px; }
.overlay.open { display: flex; }
.modal { background: var(--surface); border-radius: var(--radius); width: 680px; max-width: 100%; box-shadow: var(--shadow-md); margin: auto; }
.modal-wide { width: 820px; }
.mhd { padding: 20px 22px 16px; border-bottom: 1px solid var(--border); display: flex; align-items: center; justify-content: space-between; }
.mhd-t { font-size: 16px; font-weight: 700; color: var(--text1); }
.mhd-sub { font-size: 12px; color: var(--text3); margin-top: 2px; }
.mbody { padding: 22px; display: flex; flex-direction: column; gap: 18px; }
.mft { padding: 16px 22px; border-top: 1px solid var(--border); display: flex; gap: 10px; justify-content: flex-end; }
.btn-cancel { padding: 9px 20px; border-radius: var(--radius-sm); border: 1px solid var(--border2); background: var(--surface); font-size: 13.5px; color: var(--text2); cursor: pointer; font-family: var(--font); }
.btn-cancel:hover { background: var(--surface2); }
.btn-save { padding: 9px 24px; border-radius: var(--radius-sm); border: none; background: var(--accent); color: #fff; font-size: 13.5px; cursor: pointer; font-weight: 700; font-family: var(--font); }
.btn-save:hover { background: var(--accent-d); }

/* ═══ FORM ELEMENTS ═══════════════════════════════════════════════ */
.fg { display: flex; flex-direction: column; gap: 5px; }
.fg label { font-size: 12px; font-weight: 600; color: var(--text2); }
.fg label .req { color: var(--red); }
.fi { width: 100%; padding: 9px 12px; border: 1.5px solid var(--border2); border-radius: var(--radius-sm); font-size: 13.5px; font-family: var(--font); color: var(--text1); background: var(--surface); outline: none; transition: border-color 0.15s; }
.fi:focus { border-color: var(--accent); }
.fi.err { border-color: var(--red); background: #fff8f8; }
.fi[readonly] { background: var(--surface2); color: var(--text2); cursor: default; }
textarea.fi { resize: vertical; min-height: 80px; }
.frow { display: grid; grid-template-columns: 1fr 1fr; gap: 14px; }
.frow3 { display: grid; grid-template-columns: 1fr 1fr 1fr; gap: 14px; }

/* ═══ SECTION CARDS (New Task Modal) ═════════════════════════════ */
.sec-card { border-radius: var(--radius); border: 1.5px solid; padding: 18px; display: flex; flex-direction: column; gap: 14px; }
.sec-card.client-card { border-color: var(--client-c); background: linear-gradient(135deg, var(--client-light) 0%, rgba(227,240,250,0.3) 100%); }
.sec-card.project-card { border-color: var(--project-c); background: linear-gradient(135deg, var(--project-light) 0%, rgba(225,245,236,0.3) 100%); }
.sec-card.exec-card { border-color: var(--exec-c); background: linear-gradient(135deg, var(--exec-light) 0%, rgba(250,238,224,0.3) 100%); }
.sec-card-header { display: flex; align-items: center; gap: 10px; margin-bottom: 2px; }
.sec-card-icon { width: 34px; height: 34px; border-radius: 9px; display: flex; align-items: center; justify-content: center; }
.sec-card-icon i { font-size: 18px; }
.sec-card.client-card .sec-card-icon { background: var(--client-c); color: #fff; }
.sec-card.project-card .sec-card-icon { background: var(--project-c); color: #fff; }
.sec-card.exec-card .sec-card-icon { background: var(--exec-c); color: #fff; }
.sec-card-title { font-size: 13px; font-weight: 700; }
.sec-card.client-card .sec-card-title { color: var(--client-c); }
.sec-card.project-card .sec-card-title { color: var(--project-c); }
.sec-card.exec-card .sec-card-title { color: var(--exec-c); }

/* ═══ FILE UPLOAD ═════════════════════════════════════════════════ */
.file-drop { border: 2px dashed var(--border2); border-radius: var(--radius-sm); padding: 20px; text-align: center; cursor: pointer; transition: border-color 0.15s; }
.file-drop:hover { border-color: var(--accent); }
.file-drop i { font-size: 28px; color: var(--text3); margin-bottom: 8px; display: block; }
.file-drop span { font-size: 12px; color: var(--text3); }
.file-list { display: flex; flex-wrap: wrap; gap: 6px; margin-top: 8px; }
.file-chip { display: flex; align-items: center; gap: 5px; padding: 4px 10px; background: var(--surface); border: 1px solid var(--border); border-radius: 20px; font-size: 11px; color: var(--text2); }
.file-chip button { background: none; border: none; cursor: pointer; color: var(--text3); font-size: 14px; line-height: 1; padding: 0; }

/* ═══ PAYMENT ROW ═════════════════════════════════════════════════ */
.payment-row { display: flex; gap: 8px; align-items: center; }
.payment-row .fi { flex: 1; }

/* ═══ FINANCE CARD ════════════════════════════════════════════════ */
.fin2-hero{background:linear-gradient(135deg,#1C1A3A 0%,#534AB7 100%);border-radius:var(--radius);padding:22px 24px;margin-bottom:20px;color:#fff;}
.fin2-hero-top{display:flex;align-items:center;justify-content:space-between;gap:12px;flex-wrap:wrap;margin-bottom:18px;}
.fin2-hero-title{font-size:18px;font-weight:700;}
.fin2-hero-sub{font-size:11px;opacity:.7;margin-top:2px;}
.fin2-kpis{display:grid;grid-template-columns:repeat(5,1fr);gap:12px;}
.fin2-kpi{background:rgba(255,255,255,.12);border-radius:10px;padding:14px 16px;}
.fin2-kpi-lbl{font-size:10px;opacity:.8;margin-bottom:5px;}
.fin2-kpi-val{font-size:20px;font-weight:700;line-height:1;}
.fin2-kpi-sub{font-size:10px;opacity:.65;margin-top:3px;}
.fin2-kpi.pos{background:rgba(29,158,117,.25);}
.fin2-kpi.neg{background:rgba(226,75,74,.25);}
.fin2-kpi.warn{background:rgba(239,159,39,.25);}
@media(max-width:900px){.fin2-kpis{grid-template-columns:1fr 1fr;}}

.fin2-client-card{background:var(--surface);border:1px solid var(--border);border-radius:var(--radius);box-shadow:var(--shadow);overflow:hidden;}
.fin2-cc-header{display:flex;align-items:center;justify-content:space-between;gap:10px;padding:16px 18px 12px;border-bottom:1px solid var(--border);}
.fin2-cc-name{font-size:14px;font-weight:700;color:var(--text1);}
.fin2-cc-code{font-size:11px;color:var(--text3);margin-top:1px;}
.fin2-cc-kpis{display:grid;grid-template-columns:repeat(3,1fr);gap:0;border-bottom:1px solid var(--border);}
.fin2-cc-kpi{padding:12px 14px;border-left:1px solid var(--border);text-align:center;}
.fin2-cc-kpi:last-child{border-left:none;}
.fin2-cc-kpi-lbl{font-size:10px;color:var(--text3);margin-bottom:3px;}
.fin2-cc-kpi-val{font-size:14px;font-weight:700;color:var(--text1);}
.fin2-cc-projects{padding:10px 18px 4px;}
.fin2-cc-proj-row{display:flex;align-items:center;justify-content:space-between;gap:8px;padding:7px 0;border-bottom:1px solid var(--border);cursor:pointer;transition:background .1s;}
.fin2-cc-proj-row:hover{background:var(--surface2);margin:0 -18px;padding:7px 18px;}
.fin2-cc-proj-row:last-child{border-bottom:none;}
.fin2-cc-proj-info{display:flex;align-items:center;gap:8px;}
.fin2-cc-proj-code{font-size:11px;font-weight:700;color:var(--accent);font-family:monospace;}
.fin2-cc-proj-desc{font-size:12px;color:var(--text2);max-width:160px;white-space:nowrap;overflow:hidden;text-overflow:ellipsis;}
.fin2-cc-proj-amounts{display:flex;align-items:center;gap:10px;font-size:11px;}
.fin2-cc-paid{color:var(--green);font-weight:600;}
.fin2-cc-rem{color:var(--red);font-weight:600;}
.fin2-cc-footer{padding:10px 18px;display:flex;gap:8px;background:var(--surface2);}

.pfin-kpis{display:grid;grid-template-columns:repeat(5,1fr);gap:10px;padding:16px 22px;background:var(--surface2);border-bottom:1px solid var(--border);}
.pfin-kpi{background:var(--surface);border:1px solid var(--border);border-radius:var(--radius-sm);padding:12px 14px;text-align:center;}
.pfin-kpi-lbl{font-size:10px;color:var(--text3);margin-bottom:4px;}
.pfin-kpi-val{font-size:15px;font-weight:700;color:var(--text1);line-height:1;}
.pfin-kpi.kpi-green{border-color:var(--green);background:var(--green-light);}
.pfin-kpi.kpi-red  {border-color:var(--red);background:var(--red-light);}
.pfin-kpi.kpi-blue {border-color:var(--blue);background:var(--blue-light);}
.pfin-kpi.kpi-amber{border-color:var(--amber);background:var(--amber-light);}
.pfin-kpi.kpi-acc  {border-color:var(--accent);background:var(--accent-light);}
.pfin-kpi .kpi-green-val{color:var(--green);}
.pfin-kpi .kpi-red-val  {color:var(--red);}
.pfin-kpi .kpi-blue-val {color:var(--blue);}
.pfin-kpi .kpi-amber-val{color:var(--amber);}
.pfin-kpi .kpi-acc-val  {color:var(--accent);}
@media(max-width:900px){.pfin-kpis{grid-template-columns:1fr 1fr;}}

.pfin-actions{display:flex;gap:8px;padding:12px 22px;border-bottom:1px solid var(--border);background:var(--surface2);flex-wrap:wrap;}
.pfin-btn{display:inline-flex;align-items:center;gap:6px;padding:8px 16px;border-radius:var(--radius-sm);font-size:13px;font-weight:600;cursor:pointer;border:none;font-family:var(--font);transition:all .12s;}
.pfin-btn-income{background:var(--green);color:#fff;}
.pfin-btn-income:hover{background:#16876a;}
.pfin-btn-expense{background:var(--red);color:#fff;}
.pfin-btn-expense:hover{background:#c73939;}
.pfin-btn-print{background:var(--surface);color:var(--text2);border:1px solid var(--border2);}
.pfin-btn-print:hover{background:var(--surface2);}
.pfin-btn-export{background:var(--accent);color:#fff;}
.pfin-btn-export:hover{background:var(--accent-d);}

.pfin-tabs{display:flex;gap:0;padding:0 22px;border-bottom:1px solid var(--border);}
.pfin-tab{padding:10px 18px;font-size:13px;font-weight:600;color:var(--text3);cursor:pointer;border-bottom:2px solid transparent;transition:all .12s;}
.pfin-tab.on{color:var(--accent);border-bottom-color:var(--accent);}
.pfin-tab:hover{color:var(--text1);}

.pfin-ledger{overflow-x:auto;}
.pfin-ledger table{width:100%;border-collapse:collapse;font-size:12.5px;}
.pfin-ledger th{background:var(--surface2);padding:8px 14px;font-size:10.5px;font-weight:700;color:var(--text3);text-transform:uppercase;letter-spacing:.3px;text-align:right;border-bottom:1px solid var(--border);}
.pfin-ledger td{padding:11px 14px;border-bottom:1px solid var(--border);vertical-align:middle;}
.pfin-ledger tr:last-child td{border-bottom:none;}
.pfin-ledger tr:hover td{background:var(--surface2);}
.pfin-row-income{border-right:3px solid var(--green);}
.pfin-row-expense{border-right:3px solid var(--red);}
.pfin-amount-income{color:var(--green);font-weight:700;font-size:13px;}
.pfin-amount-expense{color:var(--red);font-weight:700;font-size:13px;}
.pfin-balance{font-weight:700;font-family:monospace;}
.pfin-cat-badge{display:inline-flex;align-items:center;gap:4px;padding:2px 8px;border-radius:12px;font-size:10px;font-weight:600;background:var(--surface3);color:var(--text2);}
.pfin-receipt-thumb{width:32px;height:32px;object-fit:cover;border-radius:4px;border:1px solid var(--border);cursor:pointer;}

.fin-quick-modal .mbody{gap:14px;}
.fin-amount-big input{font-size:24px;font-weight:700;text-align:center;color:var(--accent);}
.expense-cat-grid{display:grid;grid-template-columns:repeat(4,1fr);gap:8px;margin-top:4px;}
.exp-cat-btn{display:flex;flex-direction:column;align-items:center;gap:4px;padding:10px 6px;border-radius:var(--radius-sm);border:1.5px solid var(--border);background:var(--surface);cursor:pointer;font-size:11px;color:var(--text2);transition:all .12s;font-family:var(--font);}
.exp-cat-btn:hover{border-color:var(--accent);background:var(--accent-light);color:var(--accent);}
.exp-cat-btn.sel{border-color:var(--accent);background:var(--accent);color:#fff;}
.exp-cat-btn .cat-icon{font-size:20px;}

.receipt-drop{border:2px dashed var(--border2);border-radius:var(--radius-sm);padding:14px;text-align:center;cursor:pointer;transition:border-color .15s;background:var(--surface2);}
.receipt-drop:hover{border-color:var(--accent);}
.receipt-drop i{font-size:24px;color:var(--text3);display:block;margin-bottom:4px;}
.receipt-drop span{font-size:11.5px;color:var(--text3);}
.receipt-preview-wrap{margin-top:8px;display:flex;align-items:center;gap:10px;}
.receipt-preview-wrap img{width:72px;height:72px;object-fit:cover;border-radius:6px;border:1px solid var(--border);}

.cfin-proj-table{width:100%;border-collapse:collapse;font-size:12.5px;}
.cfin-proj-table th{background:var(--surface2);padding:8px 12px;font-size:10px;font-weight:700;color:var(--text3);text-transform:uppercase;text-align:right;border-bottom:1px solid var(--border);}
.cfin-proj-table td{padding:10px 12px;border-bottom:1px solid var(--border);vertical-align:middle;}
.cfin-proj-table tr:hover td{background:var(--surface2);}

/* ═══ REPORT CARD ═════════════════════════════════════════════════ */
.report-card { background: var(--surface); border: 1px solid var(--border); border-radius: var(--radius); padding: 16px; box-shadow: var(--shadow); }
.rc-header { display: flex; justify-content: space-between; align-items: flex-start; margin-bottom: 10px; }
.rc-task { font-size: 13px; font-weight: 700; color: var(--text1); }
.rc-proj { font-size: 11px; color: var(--text3); margin-top: 2px; }
.rc-content { font-size: 12px; color: var(--text2); background: var(--surface2); padding: 10px; border-radius: var(--radius-sm); margin: 10px 0; line-height: 1.6; }
.rc-stages { font-size: 11px; color: var(--text3); line-height: 1.7; }

/* ═══ CLIENT / PROJECT CARDS GRID ════════════════════════════════ */
.cards-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(280px, 1fr)); gap: 14px; }
.entity-card { background: var(--surface); border: 1px solid var(--border); border-radius: var(--radius); padding: 18px; box-shadow: var(--shadow); }
.ec-top { display: flex; align-items: center; justify-content: space-between; margin-bottom: 12px; }
.ec-name { font-size: 14px; font-weight: 700; color: var(--text1); }
.ec-code { font-size: 11px; color: var(--text3); margin-top: 2px; }
.ec-meta { display: flex; flex-direction: column; gap: 5px; margin-top: 10px; }
.ec-meta-row { display: flex; align-items: center; justify-content: space-between; font-size: 12px; }
.ec-meta-key { color: var(--text3); }
.ec-meta-val { font-weight: 600; color: var(--text1); }

/* ═══ ENGINEER TASK CARD ══════════════════════════════════════════ */
.eng-task-card { background: var(--surface); border: 1px solid var(--border); border-radius: var(--radius); padding: 16px 18px; box-shadow: var(--shadow); margin-bottom: 10px; }
.etc-header { display: flex; align-items: center; gap: 10px; margin-bottom: 12px; }
.etc-code { font-size: 12px; font-weight: 700; color: var(--text3); }
.etc-name { flex: 1; font-size: 14px; font-weight: 600; color: var(--text1); }
.etc-body { display: grid; grid-template-columns: 1fr 1fr; gap: 10px; margin-bottom: 12px; }
.etc-field { font-size: 12px; }
.etc-field-lbl { color: var(--text3); margin-bottom: 2px; }
.etc-field-val { font-weight: 600; color: var(--text1); }
.etc-progress { margin-top: 8px; }
.etc-prog-top { display: flex; justify-content: space-between; font-size: 11px; margin-bottom: 4px; }

/* ═══ SETTINGS ════════════════════════════════════════════════════ */
.settings-card { background: var(--surface); border: 1px solid var(--border); border-radius: var(--radius); padding: 22px; margin-bottom: 14px; box-shadow: var(--shadow); }
.settings-card h3 { font-size: 14px; font-weight: 700; margin-bottom: 16px; color: var(--text1); display: flex; align-items: center; gap: 8px; }
.settings-card h3 i { font-size: 18px; color: var(--accent); }

/* ═══ EMPTY STATE ═════════════════════════════════════════════════ */
.empty { text-align: center; padding: 50px 20px; color: var(--text3); }
.empty i { font-size: 40px; display: block; margin-bottom: 12px; opacity: 0.5; }
.empty p { font-size: 13px; }

/* ═══ TOAST ═══════════════════════════════════════════════════════ */
.toast { position: fixed; bottom: 24px; right: 24px; background: var(--text1); color: #e8e8e4; font-size: 13px; padding: 11px 18px; border-radius: var(--radius-sm); z-index: 900; opacity: 0; transition: opacity 0.25s, transform 0.25s; transform: translateY(8px); pointer-events: none; max-width: 340px; }
.toast.show { opacity: 1; transform: translateY(0); }

/* ═══ SCROLLBAR ═══════════════════════════════════════════════════ */
::-webkit-scrollbar { width: 5px; height: 5px; }
::-webkit-scrollbar-track { background: transparent; }
::-webkit-scrollbar-thumb { background: var(--border2); border-radius: 3px; }

/* ═══ RESPONSIVE ══════════════════════════════════════════════════ */
@media(max-width:900px){
  .sidebar { width: 58px; }
  .sb-brand .sb-mark + * { display: none; }
  .ni span, .ni .nbadge, .sb-nav .sb-sec, .sb-user .user-info { display: none; }
  .ni { padding: 10px; justify-content: center; }
  .ni.on::before { top: auto; bottom: 0; right: 0; width: 100%; height: 3px; border-radius: 3px 3px 0 0; }
  .stats-row { grid-template-columns: 1fr 1fr; }
  .frow { grid-template-columns: 1fr; }
  .frow3 { grid-template-columns: 1fr; }
  .fin2-kpis, .pfin-kpis { grid-template-columns: 1fr 1fr; }
}

/* ═══ REPORTS — ENHANCED ═════════════════════════════════════════ */
.rep-hero {
  background: linear-gradient(135deg, #1A3A1C 0%, #1A8A5A 100%);
  border-radius: var(--radius); padding: 20px 24px; margin-bottom: 18px;
  color: #fff; display: flex; align-items: center; justify-content: space-between; gap: 16px; flex-wrap: wrap;
}
.rep-hero-title { font-size: 17px; font-weight: 700; margin-bottom: 2px; }
.rep-hero-sub   { font-size: 11px; opacity: 0.75; }
.rep-stat-pills { display: flex; gap: 10px; flex-wrap: wrap; }
.rep-stat-pill  {
  background: rgba(255,255,255,0.15); border-radius: 20px; padding: 6px 14px;
  font-size: 12px; display: flex; align-items: center; gap: 6px;
}
.rep-stat-pill strong { font-size: 15px; font-weight: 700; }

/* Report card */
.rep-card {
  background: var(--surface); border: 1px solid var(--border);
  border-radius: var(--radius); box-shadow: var(--shadow);
  display: flex; flex-direction: column; overflow: hidden;
  transition: box-shadow 0.14s, transform 0.14s; cursor: pointer;
}
.rep-card:hover { box-shadow: var(--shadow-md); transform: translateY(-1px); }

.rep-card-top {
  padding: 14px 16px 10px; display: flex;
  align-items: flex-start; justify-content: space-between; gap: 8px;
}
.rep-type-badge {
  display: inline-flex; align-items: center; gap: 5px;
  padding: 4px 10px; border-radius: 20px; font-size: 11px; font-weight: 700;
}
.rep-type-daily     { background: #FCE4EC; color: #C2185B; }
.rep-type-weekly    { background: #E3F2FD; color: #1565C0; }
.rep-type-milestone { background: #E8F5E9; color: #1B5E20; }
.rep-type-final     { background: #FFF3E0; color: #E65100; }

.rep-num  { font-size: 10px; font-weight: 700; color: var(--text3); font-family: monospace; }
.rep-date { font-size: 10px; color: var(--text3); }

.rep-proj-name { padding: 0 16px 4px; font-size: 13px; font-weight: 700; color: var(--text1); }
.rep-proj-code { padding: 0 16px 10px; font-size: 11px; color: var(--text3); display: flex; align-items: center; gap: 6px; }

.rep-prog-row { padding: 8px 16px 10px; border-top: 1px solid var(--border); }
.rep-prog-label { display: flex; justify-content: space-between; font-size: 11px; color: var(--text3); margin-bottom: 5px; }
.rep-prog-label strong { color: var(--accent); font-size: 13px; }

.rep-content-preview {
  padding: 0 16px 10px; font-size: 12px; color: var(--text2);
  line-height: 1.65; display: -webkit-box; -webkit-line-clamp: 3;
  -webkit-box-orient: vertical; overflow: hidden;
}

.rep-footer {
  padding: 10px 16px; border-top: 1px solid var(--border);
  display: flex; align-items: center; justify-content: space-between; gap: 8px;
  background: var(--surface2); margin-top: auto;
}
.rep-eng-tag { display: flex; align-items: center; gap: 5px; font-size: 11px; color: var(--text3); }
.rep-eng-tag i { font-size: 13px; }
.rep-files-tag { display: flex; align-items: center; gap: 4px; font-size: 11px; color: var(--accent); font-weight: 600; }
.rep-files-tag i { font-size: 13px; }

/* Report Detail Modal */
.rep-detail-header {
  display: flex; align-items: flex-start; justify-content: space-between;
  gap: 12px; margin-bottom: 20px; padding-bottom: 16px; border-bottom: 1px solid var(--border);
}
.rep-detail-meta { display: flex; flex-wrap: wrap; gap: 8px; margin-bottom: 14px; }
.rep-detail-tag {
  display: flex; align-items: center; gap: 5px; padding: 4px 10px;
  background: var(--surface2); border-radius: 20px; font-size: 11px; color: var(--text2);
}
.rep-detail-tag i { font-size: 13px; color: var(--accent); }
.rep-detail-tag strong { color: var(--text1); }

.rep-detail-section { margin-bottom: 16px; }
.rep-detail-section-title {
  font-size: 11px; font-weight: 700; color: var(--text3); text-transform: uppercase;
  letter-spacing: 0.5px; margin-bottom: 7px; display: flex; align-items: center; gap: 6px;
}
.rep-detail-section-title i { font-size: 14px; color: var(--accent); }
.rep-detail-content {
  background: var(--surface2); border-radius: var(--radius-sm);
  padding: 12px 14px; font-size: 13px; color: var(--text1); line-height: 1.7;
  border-right: 3px solid var(--accent-mid);
}
.rep-detail-attachments { display: flex; flex-wrap: wrap; gap: 8px; }
.rep-att-chip {
  display: flex; align-items: center; gap: 6px; padding: 6px 12px;
  background: var(--surface2); border: 1px solid var(--border);
  border-radius: var(--radius-sm); font-size: 12px; color: var(--text1);
  cursor: pointer; text-decoration: none; transition: background 0.12s;
}
.rep-att-chip:hover { background: var(--accent-light); color: var(--accent); }
.rep-att-chip i { font-size: 16px; color: var(--accent); }
.rep-att-img-preview {
  width: 80px; height: 80px; object-fit: cover; border-radius: var(--radius-sm);
  border: 1px solid var(--border); cursor: pointer;
}

/* Modal file drop in report form */
.rep-file-drop {
  border: 2px dashed var(--border2); border-radius: var(--radius-sm);
  padding: 18px; text-align: center; cursor: pointer; transition: border-color 0.15s;
  background: var(--surface2);
}
.rep-file-drop:hover { border-color: var(--project-c); background: var(--project-light); }
.rep-file-drop i { font-size: 26px; color: var(--text3); display: block; margin-bottom: 6px; }
.rep-file-drop span { font-size: 12px; color: var(--text3); }

.rep-form-preview {
  display: flex; flex-wrap: wrap; gap: 6px; margin-top: 8px;
}
.rep-form-file-chip {
  display: flex; align-items: center; gap: 5px; padding: 4px 10px;
  background: var(--surface); border: 1px solid var(--border);
  border-radius: 16px; font-size: 11px; color: var(--text2);
}
.rep-form-file-chip .img-thumb {
  width: 28px; height: 28px; object-fit: cover;
  border-radius: 4px; border: 1px solid var(--border);
}
.rep-form-file-chip button {
  background: none; border: none; cursor: pointer;
  color: var(--text3); font-size: 14px; padding: 0; line-height: 1;
}
.rep-form-file-chip button:hover { color: var(--red); }

/* Progress display in form */
.rep-prog-display {
  display: flex; align-items: center; gap: 10px; margin-top: 6px;
}
.rep-prog-display .prog-bar { flex: 1; height: 8px; }
.rep-prog-pct-badge {
  font-size: 15px; font-weight: 700; color: var(--accent);
  min-width: 42px; text-align: left;
}


/* ═══ WORKFORCE FINANCE CARDS ══════════════════════════════════ */
.wf-cards-strip {
  display: grid; grid-template-columns: repeat(3,1fr);
  gap: 10px; padding: 12px 22px; background: var(--surface2);
  border-bottom: 1px solid var(--border); flex-shrink: 0;
}
.wf-card {
  background: var(--surface); border: 1px solid var(--border);
  border-radius: var(--radius-sm); padding: 12px 14px;
}
.wf-card-title {
  font-size: 11px; font-weight: 700; color: var(--text3);
  text-transform: uppercase; letter-spacing: .4px;
  margin-bottom: 8px; display: flex; align-items: center; gap: 5px;
}
.wf-card-row {
  display: flex; justify-content: space-between; align-items: center;
  font-size: 12px; padding: 3px 0; border-bottom: 1px solid var(--border);
}
.wf-card-row:last-child { border-bottom: none; }
.wf-card-lbl { color: var(--text3); }
.wf-card-val { font-weight: 700; color: var(--text1); }
.wf-card-val.green { color: var(--green); }
.wf-card-val.red   { color: var(--red); }
.wf-card-val.amber { color: var(--amber); }
@media(max-width:700px){ .wf-cards-strip{ grid-template-columns:1fr; } }

/* Improved workforce tables */
.wf-table-wrap { overflow-x: auto; -webkit-overflow-scrolling: touch; }
.wf-table {
  width: 100%; border-collapse: collapse;
  font-size: 12.5px; min-width: 900px;
}
.wf-table th {
  background: #f3f4f6; padding: 8px 10px; border: 1px solid #e5e7eb;
  white-space: nowrap; font-size: 11px; font-weight: 700;
  color: #6b7280; text-align: right; position: sticky; top: 0;
}
.wf-table td {
  border: 1px solid #e5e7eb; padding: 2px;
  vertical-align: middle;
}
.wf-table td input, .wf-table td select {
  width: 100%; border: none; padding: 6px 8px;
  background: transparent; font-size: 12.5px;
  font-family: inherit; box-sizing: border-box;
}
.wf-table td input:focus, .wf-table td select:focus {
  outline: 2px solid var(--accent); background: #fff; border-radius: 3px;
}
.wf-table .td-num input { text-align: left; }
.wf-table .td-calc {
  background: var(--surface2); font-weight: 700;
  font-size: 12.5px; padding: 6px 10px; white-space: nowrap; color: var(--accent);
}
.wf-table .td-paid { background: #f0fdf4; font-weight: 700; color: var(--green); padding:6px 10px; }
.wf-table .td-rem  { font-weight: 700; padding:6px 10px; }
.wf-pay-btn {
  display: inline-flex; align-items: center; gap: 3px;
  padding: 4px 8px; border-radius: 5px; border: 1px solid var(--green);
  background: var(--green-light); color: var(--green);
  font-size: 11px; cursor: pointer; font-family: var(--font); white-space: nowrap;
}
.wf-pay-btn:hover { background: var(--green); color: #fff; }
.wf-pay-chip {
  display: inline-block; font-size: 10px; padding: 2px 6px;
  border-radius: 10px; background: var(--green-light);
  color: #0a5c3f; font-weight: 600; margin: 1px;
}


/* ═══ FINANCE: WORKSHOPS & WORKERS CARDS ═══════════════════════ */
.fin-sec-tabs {
  display:flex; gap:4px; background:var(--surface3);
  padding:4px; border-radius:var(--radius-sm); flex-shrink:0;
}
.fin-sec-tab {
  padding:7px 16px; border-radius:6px; font-size:12.5px; font-weight:600;
  cursor:pointer; border:none; background:transparent; color:var(--text2);
  font-family:var(--font); transition:all .13s; white-space:nowrap;
  display:flex; align-items:center; gap:5px;
}
.fin-sec-tab.on { background:var(--surface); color:var(--accent); box-shadow:0 1px 4px rgba(0,0,0,.09); }
.fin-ws-card, .fin-wk-card {
  background:var(--surface); border:1px solid var(--border);
  border-radius:var(--radius); box-shadow:var(--shadow); overflow:hidden;
}
.fin-ws-header, .fin-wk-header {
  display:flex; align-items:flex-start; justify-content:space-between;
  gap:10px; padding:14px 18px 10px; border-bottom:1px solid var(--border);
}
.fin-ws-name { font-size:14px; font-weight:700; color:var(--text1); }
.fin-ws-meta { font-size:11px; color:var(--text3); margin-top:3px; line-height:1.6; }
.fin-ws-kpis {
  display:grid; grid-template-columns:repeat(4,1fr); gap:0;
  border-bottom:1px solid var(--border);
}
.fin-ws-kpi { padding:10px 14px; border-left:1px solid var(--border); text-align:center; }
.fin-ws-kpi:last-child { border-left:none; }
.fin-ws-kpi-lbl { font-size:10px; color:var(--text3); margin-bottom:3px; }
.fin-ws-kpi-val { font-size:13px; font-weight:700; color:var(--text1); }
.fin-pay-ledger { padding:10px 18px; }
.fin-pay-ledger-title {
  font-size:11px; font-weight:700; color:var(--text3); text-transform:uppercase;
  letter-spacing:.4px; margin-bottom:8px; display:flex; align-items:center; gap:6px;
}
.fin-pay-row {
  display:flex; align-items:center; justify-content:space-between; gap:8px;
  padding:6px 0; border-bottom:1px solid var(--border); font-size:12px;
}
.fin-pay-row:last-child { border-bottom:none; }
.fin-pay-num  { width:22px; height:22px; background:var(--accent); color:#fff; border-radius:50%; display:flex; align-items:center; justify-content:center; font-size:10px; font-weight:700; flex-shrink:0; }
.fin-pay-type { font-size:10px; padding:2px 7px; border-radius:10px; background:var(--surface2); color:var(--text2); font-weight:600; }
.fin-pay-date { color:var(--text3); font-size:11px; }
.fin-pay-amt  { font-weight:700; color:var(--green); }
.fin-pay-rem  { font-size:11px; color:var(--text3); }
.fin-pay-method { font-size:10px; color:var(--text3); }
.fin-ws-footer, .fin-wk-footer {
  padding:10px 18px; display:flex; align-items:center; justify-content:space-between;
  background:var(--surface2); gap:8px; flex-wrap:wrap;
}
.fin-add-pay-btn {
  display:inline-flex; align-items:center; gap:6px;
  padding:7px 14px; border-radius:var(--radius-sm);
  background:var(--green); color:#fff; border:none;
  font-size:12.5px; font-weight:600; cursor:pointer; font-family:var(--font);
  transition:background .12s;
}
.fin-add-pay-btn:hover { background:#16876a; }
.fin-prog-inline {
  display:flex; align-items:center; gap:6px; font-size:11px; color:var(--text3);
}
.fin-prog-inline .prog-bar { width:80px; height:6px; }
/* WK card — 3 kpis */
.fin-wk-kpis { display:grid; grid-template-columns:repeat(3,1fr); gap:0; border-bottom:1px solid var(--border); }
.fin-wk-kpi  { padding:10px 14px; border-left:1px solid var(--border); text-align:center; }
.fin-wk-kpi:last-child { border-left:none; }
.fin-wk-kpi-lbl { font-size:10px; color:var(--text3); margin-bottom:3px; }
.fin-wk-kpi-val { font-size:13px; font-weight:700; color:var(--text1); }
/* Payment form inline */
.fin-pay-form {
  padding:10px 18px 14px; background:#f9fafb; border-top:1px solid var(--border);
  display:none;
}
.fin-pay-form.show { display:block; }


/* ═══ PROJECT ACTION BUTTONS ════════════════════════════════════ */
.proj-action-row {
  display: flex; gap: 8px; align-items: center; flex-wrap: wrap;
}
.proj-btn {
  display: inline-flex; align-items: center; gap: 8px;
  padding: 10px 18px; border-radius: var(--radius-sm);
  font-size: 13.5px; font-weight: 700; cursor: pointer;
  border: 1.5px solid transparent; font-family: var(--font);
  transition: all .15s; white-space: nowrap; line-height: 1;
  min-height: 40px; letter-spacing: .01em;
}
.proj-btn i { font-size: 17px; flex-shrink: 0; }
.proj-btn-edit {
  background: var(--accent-light); color: var(--accent);
  border-color: var(--accent-mid);
}
.proj-btn-edit:hover { background: var(--accent); color: #fff; border-color: var(--accent); }
.proj-btn-follow {
  background: var(--blue-light); color: var(--blue);
  border-color: #90bfee;
}
.proj-btn-follow:hover { background: var(--blue); color: #fff; border-color: var(--blue); }
.proj-btn-del {
  background: var(--red-light); color: var(--red);
  border-color: #f0a5a5;
}
.proj-btn-del:hover { background: var(--red); color: #fff; border-color: var(--red); }


/* ═══ DAILY SITE LOG — ISSUES & SUBMIT ═════════════════════════ */
.log-submit-bar {
  display:flex; align-items:center; justify-content:space-between;
  gap:10px; margin-top:14px; padding:12px 14px;
  background:linear-gradient(135deg,#f0fdf4,#dcfce7);
  border:1.5px solid #86efac; border-radius:var(--radius-sm);
  flex-wrap:wrap;
}
.log-status-badge {
  display:inline-flex; align-items:center; gap:5px;
  padding:4px 10px; border-radius:12px; font-size:11px; font-weight:700;
}
.log-status-draft     { background:#fef3c7; color:#92400e; }
.log-status-submitted { background:#d1fae5; color:#065f46; }
.log-submit-btn {
  display:inline-flex; align-items:center; gap:7px;
  padding:9px 20px; background:var(--green); color:#fff;
  border:none; border-radius:var(--radius-sm); font-size:13px;
  font-weight:700; cursor:pointer; font-family:var(--font);
  transition:background .13s;
}
.log-submit-btn:hover  { background:#16876a; }
.log-submit-btn:disabled { opacity:.5; cursor:not-allowed; }
/* Issues */
.log-issue-card {
  background:var(--surface); border:1px solid var(--border);
  border-radius:var(--radius-sm); padding:10px 12px; margin:6px 0;
  border-right:3px solid var(--amber);
}
.log-issue-card.pri-high   { border-right-color:var(--red); }
.log-issue-card.pri-low    { border-right-color:var(--green); }
.issue-status-badge {
  display:inline-flex; align-items:center; gap:3px;
  padding:2px 8px; border-radius:10px; font-size:10px; font-weight:700;
  background:var(--surface2); color:var(--text2);
}
/* Daily log report card in reports section */
.dl-report-card {
  background:var(--surface); border:1px solid var(--border);
  border-radius:var(--radius); box-shadow:var(--shadow);
  overflow:hidden; display:flex; flex-direction:column;
}
.dl-report-header {
  padding:12px 16px 10px; border-bottom:1px solid var(--border);
  background:linear-gradient(135deg,#f8f9ff,#f0f1ff);
  display:flex; justify-content:space-between; align-items:flex-start; gap:8px;
}
.dl-report-meta { display:flex; flex-wrap:wrap; gap:6px; padding:10px 16px; }
.dl-report-meta-item { display:flex; align-items:center; gap:4px; font-size:11.5px; color:var(--text2); }
.dl-report-meta-item i { font-size:13px; color:var(--text3); }
.dl-report-body { padding:0 16px 10px; font-size:12.5px; color:var(--text2); line-height:1.6; }
.dl-report-actions {
  padding:10px 16px; border-top:1px solid var(--border);
  background:var(--surface2); display:flex; gap:6px; flex-wrap:wrap;
}
.dl-action-btn {
  display:inline-flex; align-items:center; gap:5px;
  padding:6px 12px; border-radius:var(--radius-sm); font-size:12px;
  font-weight:600; cursor:pointer; border:1px solid var(--border2);
  background:var(--surface); color:var(--text2); font-family:var(--font);
  transition:all .12s;
}
.dl-action-btn:hover { background:var(--accent); color:#fff; border-color:var(--accent); }
.dl-action-btn.green-btn { background:var(--green-light); color:var(--green); border-color:var(--green); }
.dl-action-btn.green-btn:hover { background:var(--green); color:#fff; }
/* Dashboard daily reports strip */
.dash-daily-strip { margin-top:20px; }
.dash-daily-title {
  font-size:13px; font-weight:700; color:var(--text1);
  margin-bottom:12px; display:flex; align-items:center; gap:8px;
}
.dash-dl-card {
  background:var(--surface); border:1px solid var(--border);
  border-radius:var(--radius-sm); padding:12px 16px;
  display:flex; align-items:center; gap:12px;
  transition:box-shadow .12s; cursor:default;
}
.dash-dl-card:hover { box-shadow:var(--shadow-md); }
.dash-dl-date {
  min-width:58px; text-align:center; background:var(--accent);
  color:#fff; border-radius:8px; padding:6px 4px;
  font-size:11px; font-weight:700; line-height:1.3; flex-shrink:0;
}
.dash-dl-body { flex:1; min-width:0; }
.dash-dl-proj { font-size:12px; font-weight:700; color:var(--text1); }
.dash-dl-summary { font-size:11.5px; color:var(--text3); white-space:nowrap; overflow:hidden; text-overflow:ellipsis; }


/* ═══ REPORTS GROUPING ═════════════════════════════════════════ */
.rep-group-toggle {
  display: flex; gap: 4px; background: var(--surface3);
  padding: 4px; border-radius: var(--radius-sm);
}
.rep-group-btn {
  padding: 7px 14px; border-radius: 6px; font-size: 12.5px;
  font-weight: 600; cursor: pointer; border: none;
  background: transparent; color: var(--text2);
  font-family: var(--font); transition: all .13s; white-space: nowrap;
}
.rep-group-btn.on { background: var(--surface); color: var(--accent); box-shadow: 0 1px 4px rgba(0,0,0,.09); }

.rep-group-section { margin-bottom: 18px; }
.rep-group-header {
  display: flex; align-items: center; justify-content: space-between;
  padding: 12px 16px; background: var(--surface);
  border: 1px solid var(--border); border-radius: var(--radius-sm);
  cursor: pointer; transition: background .12s; user-select: none;
  margin-bottom: 0;
}
.rep-group-header:hover { background: var(--surface2); }
.rep-group-header.open { border-radius: var(--radius-sm) var(--radius-sm) 0 0; background: var(--accent-light); border-color: var(--accent-mid); }
.rep-group-title { display: flex; align-items: center; gap: 10px; }
.rep-group-icon { width: 34px; height: 34px; border-radius: 9px; display: flex; align-items: center; justify-content: center; font-size: 17px; flex-shrink: 0; }
.rep-group-name { font-size: 14px; font-weight: 700; color: var(--text1); }
.rep-group-meta { font-size: 11px; color: var(--text3); margin-top: 2px; }
.rep-group-right { display: flex; align-items: center; gap: 10px; }
.rep-count-badge {
  display: inline-flex; align-items: center; gap: 4px;
  padding: 3px 10px; border-radius: 12px; font-size: 11px;
  font-weight: 700; background: var(--accent-light); color: var(--accent);
}
.rep-group-chevron { font-size: 16px; color: var(--text3); transition: transform .2s; }
.rep-group-body {
  border: 1px solid var(--accent-mid); border-top: none;
  border-radius: 0 0 var(--radius-sm) var(--radius-sm);
  padding: 12px; background: var(--surface2);
  display: none;
}
.rep-group-body.open { display: block; }

/* Sub-group (project inside engineer/client) */
.rep-sub-group { margin-bottom: 10px; }
.rep-sub-header {
  display: flex; align-items: center; justify-content: space-between;
  padding: 8px 12px; background: var(--surface); border: 1px solid var(--border);
  border-radius: var(--radius-sm); cursor: pointer; margin-bottom: 0;
  transition: background .12s;
}
.rep-sub-header:hover { background: var(--blue-light); }
.rep-sub-header.open { background: var(--blue-light); border-color: #90bfee; border-radius: var(--radius-sm) var(--radius-sm) 0 0; }
.rep-sub-body {
  border: 1px solid #90bfee; border-top: none;
  border-radius: 0 0 var(--radius-sm) var(--radius-sm);
  padding: 10px; background: var(--surface);
  display: none;
}
.rep-sub-body.open { display: block; }
.rep-cards-row { display: grid; grid-template-columns: repeat(auto-fill,minmax(290px,1fr)); gap: 10px; }


/* ═══ WORKSHOP FINANCE — GROUPED PROJECT CARDS ══════════════════ */
.ws-proj-card {
  background: var(--surface); border: 1.5px solid var(--border);
  border-radius: var(--radius); box-shadow: var(--shadow);
  overflow: hidden; margin-bottom: 20px;
}
.ws-proj-header {
  padding: 14px 18px 12px;
  background: linear-gradient(135deg,#1C1A3A 0%,#534AB7 100%);
  color: #fff;
}
.ws-proj-title {
  display: flex; align-items: center; gap: 10px; margin-bottom: 10px;
}
.ws-proj-name { font-size: 16px; font-weight: 700; }
.ws-proj-badges { display: flex; gap: 6px; align-items: center; flex-wrap: wrap; }
.ws-proj-edit-btn {
  display: inline-flex; align-items: center; gap: 4px;
  padding: 3px 9px; border-radius: 6px; font-size: 10px;
  font-weight: 600; cursor: pointer; border: 1px solid rgba(255,255,255,.3);
  background: rgba(255,255,255,.1); color: #fff; font-family: var(--font);
  transition: background .12s;
}
.ws-proj-edit-btn:hover { background: rgba(255,255,255,.2); }
.ws-proj-name-input {
  font-size: 15px; font-weight: 700; background: rgba(255,255,255,.15);
  border: 1px solid rgba(255,255,255,.4); border-radius: 6px;
  color: #fff; padding: 4px 10px; font-family: inherit;
  min-width: 200px;
}
/* Financial summary grid */
.ws-fin-summary {
  display: grid; grid-template-columns: repeat(5,1fr);
  gap: 0; border-top: 1px solid rgba(255,255,255,.15); padding-top: 10px;
}
.ws-fin-kpi { padding: 6px 10px; border-left: 1px solid rgba(255,255,255,.15); }
.ws-fin-kpi:first-child { border-left: none; }
.ws-fin-kpi-lbl { font-size: 9.5px; opacity: .75; margin-bottom: 3px; }
.ws-fin-kpi-val { font-size: 13px; font-weight: 700; }
@media(max-width:900px){ .ws-fin-summary{ grid-template-columns:repeat(3,1fr); } }

/* Workshop rows inside project card */
.ws-row {
  border-bottom: 1px solid var(--border);
}
.ws-row:last-child { border-bottom: none; }
.ws-row-header {
  display: flex; align-items: center; justify-content: space-between;
  padding: 11px 16px; cursor: pointer; transition: background .1s;
  gap: 8px;
}
.ws-row-header:hover { background: var(--surface2); }
.ws-row-header.expanded { background: var(--accent-light); }
.ws-row-left { display: flex; align-items: center; gap: 10px; min-width: 0; }
.ws-row-name { font-size: 13px; font-weight: 700; color: var(--text1); }
.ws-row-formula { font-size: 11px; color: var(--text3); }
.ws-row-right { display: flex; align-items: center; gap: 10px; flex-shrink: 0; }
.ws-row-kpi { text-align: center; }
.ws-row-kpi-lbl { font-size: 9px; color: var(--text3); }
.ws-row-kpi-val { font-size: 12px; font-weight: 700; }
.ws-prog-bar-sm { width: 60px; height: 5px; background: var(--border); border-radius: 3px; overflow: hidden; }
.ws-prog-fill-sm { height: 100%; background: var(--accent); border-radius: 3px; transition: width .3s; }
.ws-chevron { font-size: 14px; color: var(--text3); transition: transform .2s; }
.ws-chevron.open { transform: rotate(180deg); }

/* Expand panel */
.ws-detail-panel {
  display: none; padding: 14px 18px; background: var(--surface2);
  border-top: 1px solid var(--border);
}
.ws-detail-panel.open { display: block; }
.ws-detail-grid {
  display: grid; grid-template-columns: repeat(4,1fr); gap: 10px; margin-bottom: 14px;
}
.ws-detail-field { }
.ws-detail-lbl { font-size: 10px; color: var(--text3); margin-bottom: 2px; }
.ws-detail-val { font-size: 12.5px; font-weight: 600; color: var(--text1); }


/* ═══ SETTINGS UI ═══════════════════════════════════════════════ */
.settings-layout {
  display: grid; grid-template-columns: 200px 1fr;
  gap: 20px; align-items: start;
}
.settings-sidenav {
  background: var(--surface); border: 1px solid var(--border);
  border-radius: var(--radius); overflow: hidden; position: sticky; top: 0;
}
.set-nav-item {
  display: flex; align-items: center; gap: 9px;
  padding: 11px 16px; font-size: 13px; font-weight: 600;
  color: var(--text2); cursor: pointer; transition: all .12s;
  border-right: 3px solid transparent; border-bottom: 1px solid var(--border);
}
.set-nav-item:last-child { border-bottom: none; }
.set-nav-item:hover { background: var(--surface2); color: var(--text1); }
.set-nav-item.on { background: var(--accent-light); color: var(--accent); border-right-color: var(--accent); }
.set-nav-item i { font-size: 16px; }
.set-panel { display: none; }
.set-panel.on { display: block; }
.set-section {
  background: var(--surface); border: 1px solid var(--border);
  border-radius: var(--radius); padding: 20px 24px; margin-bottom: 16px;
}
.set-section-title {
  font-size: 14px; font-weight: 700; color: var(--text1);
  margin-bottom: 14px; display: flex; align-items: center; gap: 8px;
  padding-bottom: 10px; border-bottom: 1px solid var(--border);
}
.set-section-title i { font-size: 18px; color: var(--accent); }
.set-toggle-row {
  display: flex; align-items: center; justify-content: space-between;
  padding: 8px 0; border-bottom: 1px solid var(--border);
}
.set-toggle-row:last-child { border-bottom: none; }
.set-toggle-lbl { font-size: 13px; color: var(--text1); }
.set-toggle-sub { font-size: 11px; color: var(--text3); }
/* Toggle switch */
.toggle-sw { position: relative; width: 42px; height: 24px; flex-shrink: 0; }
.toggle-sw input { opacity: 0; width: 0; height: 0; }
.toggle-track {
  position: absolute; inset: 0; background: var(--border2);
  border-radius: 24px; cursor: pointer; transition: .2s;
}
.toggle-track:before {
  content: ''; position: absolute; height: 18px; width: 18px;
  left: 3px; bottom: 3px; background: #fff; border-radius: 50%; transition: .2s;
}
.toggle-sw input:checked + .toggle-track { background: var(--accent); }
.toggle-sw input:checked + .toggle-track:before { transform: translateX(18px); }
/* User card */
.user-card {
  display: flex; align-items: center; gap: 12px; padding: 10px 0;
  border-bottom: 1px solid var(--border);
}
.user-card:last-child { border-bottom: none; }
.user-avatar {
  width: 38px; height: 38px; border-radius: 50%; background: var(--accent);
  color: #fff; display: flex; align-items: center; justify-content: center;
  font-size: 14px; font-weight: 700; flex-shrink: 0;
}
.user-avatar.inactive { background: var(--text3); }
.user-role-badge {
  font-size: 10px; padding: 2px 8px; border-radius: 10px; font-weight: 600;
  background: var(--accent-light); color: var(--accent);
}
/* Tag list */
.tag-list { display: flex; flex-wrap: wrap; gap: 6px; margin-top: 8px; }
.tag-item {
  display: inline-flex; align-items: center; gap: 5px; padding: 4px 10px;
  background: var(--surface2); border: 1px solid var(--border); border-radius: 20px;
  font-size: 12px; color: var(--text1);
}
.tag-del {
  background: none; border: none; cursor: pointer; color: var(--text3);
  padding: 0; font-size: 14px; line-height: 1; display: flex; align-items: center;
}
.tag-del:hover { color: var(--red); }
.tag-add-row { display: flex; gap: 8px; margin-top: 8px; }
/* Activity log */
.log-row {
  display: flex; align-items: flex-start; gap: 10px; padding: 8px 0;
  border-bottom: 1px solid var(--border); font-size: 12.5px;
}
.log-dot { width: 8px; height: 8px; border-radius: 50%; background: var(--accent); flex-shrink: 0; margin-top: 5px; }
.log-time { font-size: 10.5px; color: var(--text3); white-space: nowrap; }
.log-user { font-weight: 700; color: var(--accent); }


/* ═══ ENGINEER TASKS — GROUP BY ENGINEER ════════════════════════ */
.et-view-toggle { display:flex; gap:4px; background:var(--surface3); padding:4px; border-radius:var(--radius-sm); }
.et-view-btn    { padding:7px 16px; border-radius:6px; font-size:12.5px; font-weight:600; cursor:pointer;
  border:none; background:transparent; color:var(--text2); font-family:var(--font); transition:all .13s; white-space:nowrap; }
.et-view-btn.on { background:var(--surface); color:var(--accent); box-shadow:0 1px 4px rgba(0,0,0,.09); }

.eng-group-card {
  background:var(--surface); border:1px solid var(--border);
  border-radius:var(--radius); box-shadow:var(--shadow); overflow:hidden; margin-bottom:16px;
}
.eng-group-hdr {
  display:flex; align-items:center; justify-content:space-between;
  padding:14px 18px; background:linear-gradient(135deg,#1C1A3A,#534AB7); color:#fff;
}
.eng-avatar-lg {
  width:44px; height:44px; border-radius:50%; background:rgba(255,255,255,.2);
  display:flex; align-items:center; justify-content:center;
  font-size:18px; font-weight:700; flex-shrink:0;
}
.eng-group-name { font-size:15px; font-weight:700; }
.eng-group-sub  { font-size:11px; opacity:.8; margin-top:2px; }
.eng-proj-row {
  display:flex; align-items:center; justify-content:space-between;
  padding:11px 18px; border-bottom:1px solid var(--border);
  cursor:pointer; transition:background .1s; gap:10px;
}
.eng-proj-row:last-child { border-bottom:none; }
.eng-proj-row:hover { background:var(--accent-light); }
.eng-proj-code { font-family:monospace; font-size:12px; font-weight:700; color:var(--accent); flex-shrink:0; }
.eng-proj-info { display:flex; align-items:center; gap:8px; flex:1; min-width:0; flex-wrap:wrap; }
.eng-proj-client{ font-size:12.5px; color:var(--text1); font-weight:600; }
.eng-proj-desc  { font-size:11.5px; color:var(--text3); white-space:nowrap; overflow:hidden; text-overflow:ellipsis; max-width:200px; }
.eng-proj-right { display:flex; align-items:center; gap:8px; flex-shrink:0; }
.eng-open-btn   {
  display:inline-flex; align-items:center; gap:5px;
  padding:6px 13px; border-radius:var(--radius-sm); border:1px solid var(--accent-mid);
  background:var(--accent-light); color:var(--accent); font-size:12px; font-weight:700;
  cursor:pointer; font-family:var(--font); transition:all .13s;
}
.eng-open-btn:hover { background:var(--accent); color:#fff; }
.eng-no-eng { padding:12px 18px; font-size:12px; color:var(--text3); }


/* ═══ CAMERA CAPTURE BUTTON ════════════════════════════════════ */
.fu-btn-cam {
  display: inline-flex; align-items: center; gap: 6px;
  padding: 7px 14px; border-radius: var(--radius-sm);
  background: linear-gradient(135deg,#0f766e,#0d9488);
  color: #fff; cursor: pointer; font-size: 13px; font-weight: 600;
  font-family: var(--font); border: none; transition: all .13s;
  user-select: none;
}
.fu-btn-cam:hover { background: linear-gradient(135deg,#0d9488,#0f766e); transform: scale(1.02); }
.fu-btn-cam i { font-size: 16px; }
.cam-wrap { display: inline-flex; align-items: center; gap: 8px; flex-wrap: wrap; }


/* ═══ PHOTO COMMENT CARDS ══════════════════════════════════════ */
.photo-card {
  background: var(--surface); border: 1px solid var(--border);
  border-radius: var(--radius); overflow: hidden;
  margin: 8px 0; box-shadow: var(--shadow);
}
.photo-card-img {
  width: 100%; max-height: 280px; object-fit: cover;
  display: block; cursor: zoom-in;
}
.photo-card-meta {
  display: flex; align-items: center; justify-content: space-between;
  padding: 7px 12px; background: var(--surface2);
  font-size: 11px; color: var(--text3); gap: 8px;
}
.photo-card-uploader {
  display: flex; align-items: center; gap: 6px;
}
.photo-uploader-av {
  width: 22px; height: 22px; border-radius: 50%;
  background: var(--accent); color: #fff;
  display: flex; align-items: center; justify-content: center;
  font-size: 10px; font-weight: 700; flex-shrink: 0;
}
.photo-comments {
  padding: 8px 12px; border-top: 1px solid var(--border);
}
.photo-comments-title {
  font-size: 11px; font-weight: 700; color: var(--text3);
  display: flex; align-items: center; gap: 5px; margin-bottom: 8px;
}
.photo-comment-row {
  display: flex; gap: 8px; margin-bottom: 8px; align-items: flex-start;
}
.photo-comment-av {
  width: 28px; height: 28px; border-radius: 50%; flex-shrink: 0;
  display: flex; align-items: center; justify-content: center;
  font-size: 11px; font-weight: 700; color: #fff;
  background: var(--accent);
}
.photo-comment-av.mgr { background: #534AB7; }
.photo-comment-av.eng { background: #16a34a; }
.photo-comment-bubble {
  background: var(--surface2); border-radius: 0 10px 10px 10px;
  padding: 7px 10px; flex: 1; min-width: 0;
}
.photo-comment-author {
  font-size: 11px; font-weight: 700; color: var(--accent); margin-bottom: 3px;
  display: flex; align-items: center; justify-content: space-between;
}
.photo-comment-text { font-size: 12.5px; color: var(--text1); line-height: 1.5; }
.photo-comment-time { font-size: 10px; color: var(--text3); margin-top: 3px; }
.photo-comment-del {
  background: none; border: none; cursor: pointer; color: var(--text3);
  font-size: 11px; padding: 0 2px; transition: color .1s;
}
.photo-comment-del:hover { color: var(--red); }
.photo-comment-input-row {
  display: flex; gap: 8px; margin-top: 8px; align-items: flex-end;
  border-top: 1px solid var(--border); padding-top: 8px;
}
.photo-comment-inp {
  flex: 1; border: 1px solid var(--border); border-radius: 18px;
  padding: 7px 13px; font-size: 12.5px; font-family: var(--font);
  background: var(--surface); resize: none; outline: none;
  transition: border-color .12s; min-height: 36px;
}
.photo-comment-inp:focus { border-color: var(--accent); }
.photo-comment-send {
  background: var(--accent); color: #fff; border: none;
  border-radius: 50%; width: 34px; height: 34px; flex-shrink: 0;
  display: flex; align-items: center; justify-content: center;
  cursor: pointer; font-size: 15px; transition: background .12s;
}
.photo-comment-send:hover { background: var(--accent-d); }


/* ═══════════════════════════════════════════════════════════════
   PROJECT FOLLOWUP — متابعة المشاريع
   ═══════════════════════════════════════════════════════════════ */
.pf-layout { display:grid; grid-template-columns:280px 1fr; gap:16px; height:calc(100vh - 120px); min-height:0; }
@media(max-width:860px){ .pf-layout{grid-template-columns:1fr;height:auto;} }

/* Left panel: project list */
.pf-proj-list { background:var(--surface); border:1px solid var(--border); border-radius:var(--radius); overflow-y:auto; display:flex; flex-direction:column; }
.pf-proj-search { padding:10px 12px; border-bottom:1px solid var(--border); }
.pf-proj-search input { width:100%; border:1px solid var(--border); border-radius:var(--radius-sm); padding:7px 10px; font-size:12.5px; font-family:var(--font); background:var(--surface2); }
.pf-proj-item { padding:11px 14px; border-bottom:1px solid var(--border); cursor:pointer; transition:background .1s; display:flex; align-items:flex-start; gap:8px; }
.pf-proj-item:hover { background:var(--surface2); }
.pf-proj-item.on { background:var(--accent-light); border-right:3px solid var(--accent); }
.pf-proj-code { font-family:monospace; font-size:11px; font-weight:700; color:var(--accent); }
.pf-proj-name { font-size:12.5px; font-weight:600; color:var(--text1); }
.pf-proj-meta { font-size:10.5px; color:var(--text3); margin-top:2px; }
.pf-proj-prog { width:100%; height:3px; background:var(--border); border-radius:2px; margin-top:5px; overflow:hidden; }
.pf-proj-prog-fill { height:100%; background:var(--accent); border-radius:2px; transition:width .3s; }

/* Right panel: stages */
.pf-main { overflow-y:auto; display:flex; flex-direction:column; gap:0; }
.pf-topbar { background:var(--surface); border:1px solid var(--border); border-radius:var(--radius); padding:12px 16px; margin-bottom:14px; display:flex; align-items:center; justify-content:space-between; gap:10px; flex-wrap:wrap; }
.pf-view-btns { display:flex; gap:4px; background:var(--surface3); padding:3px; border-radius:var(--radius-sm); }
.pf-view-btn { padding:5px 12px; border-radius:5px; font-size:12px; font-weight:600; cursor:pointer; border:none; background:transparent; color:var(--text2); font-family:var(--font); transition:all .12s; }
.pf-view-btn.on { background:var(--surface); color:var(--accent); box-shadow:0 1px 3px rgba(0,0,0,.1); }

/* Stage card */
.pf-stage { background:var(--surface); border:1px solid var(--border); border-radius:var(--radius); margin-bottom:12px; overflow:hidden; }
.pf-stage-header { display:flex; align-items:center; justify-content:space-between; padding:12px 16px; cursor:pointer; border-bottom:1px solid var(--border); user-select:none; }
.pf-stage-header:hover { background:var(--surface2); }
.pf-stage-name { font-size:14px; font-weight:700; color:var(--text1); display:flex; align-items:center; gap:8px; }
.pf-stage-dot { width:10px; height:10px; border-radius:50%; flex-shrink:0; }
.pf-stage-body { padding:10px 14px; }
.pf-stage-actions { display:flex; gap:6px; }

/* Task row */
.pf-task { display:flex; align-items:center; gap:10px; padding:8px 10px; border-radius:var(--radius-sm); margin-bottom:4px; cursor:pointer; transition:background .1s; border:1px solid transparent; }
.pf-task:hover { background:var(--surface2); border-color:var(--border); }
.pf-task.on { background:var(--accent-light); border-color:var(--accent-mid); }
.pf-task-status { width:10px; height:10px; border-radius:50%; flex-shrink:0; border:2px solid currentColor; }
.pf-task-name { flex:1; font-size:13px; color:var(--text1); font-weight:500; }
.pf-task-name.done { text-decoration:line-through; color:var(--text3); }
.pf-task-meta { display:flex; gap:6px; align-items:center; flex-shrink:0; flex-wrap:wrap; }
.pf-task-pill { font-size:10px; padding:2px 7px; border-radius:10px; font-weight:600; }
.pf-add-task { display:flex; align-items:center; gap:6px; padding:7px 10px; color:var(--text3); font-size:12.5px; cursor:pointer; border-radius:var(--radius-sm); transition:all .1s; border:1px dashed var(--border); margin-top:4px; }
.pf-add-task:hover { background:var(--accent-light); color:var(--accent); border-color:var(--accent); }

/* Task detail drawer */
.pf-drawer { position:fixed; top:0; left:0; width:100%; height:100%; z-index:850; display:none; }
.pf-drawer.open { display:flex; }
.pf-drawer-overlay { position:absolute; inset:0; background:rgba(0,0,0,.35); }
.pf-drawer-panel { position:absolute; left:0; top:0; height:100%; width:520px; max-width:95vw; background:var(--surface); box-shadow:-4px 0 24px rgba(0,0,0,.15); display:flex; flex-direction:column; animation:slideFromLeft .2s ease; overflow:hidden; }
@keyframes slideFromLeft { from{transform:translateX(-30px);opacity:0;} to{transform:translateX(0);opacity:1;} }
@media(max-width:600px){ .pf-drawer-panel{width:100%;top:auto;bottom:0;height:90vh;border-radius:18px 18px 0 0;animation:slideFromBottom .2s ease;} }
@keyframes slideFromBottom { from{transform:translateY(40px);opacity:0;} to{transform:translateY(0);opacity:1;} }
.pf-drawer-hdr { padding:14px 18px; border-bottom:1px solid var(--border); display:flex; align-items:flex-start; gap:10px; flex-shrink:0; }
.pf-drawer-tabs { display:flex; gap:2px; border-bottom:1px solid var(--border); padding:0 16px; flex-shrink:0; overflow-x:auto; }
.pf-dtab { padding:10px 14px; font-size:12.5px; font-weight:600; color:var(--text3); cursor:pointer; border-bottom:2px solid transparent; white-space:nowrap; }
.pf-dtab.on { color:var(--accent); border-bottom-color:var(--accent); }
.pf-drawer-body { flex:1; overflow-y:auto; padding:14px 18px; }

/* Kanban */
.pf-kanban { display:flex; gap:12px; overflow-x:auto; padding-bottom:10px; min-height:400px; }
.pf-kanban-col { min-width:240px; max-width:260px; background:var(--surface2); border-radius:var(--radius); padding:10px; flex-shrink:0; }
.pf-kanban-title { font-size:12px; font-weight:700; margin-bottom:10px; padding:4px 8px; border-radius:6px; text-align:center; }
.pf-kanban-card { background:var(--surface); border:1px solid var(--border); border-radius:var(--radius-sm); padding:10px; margin-bottom:8px; cursor:pointer; box-shadow:var(--shadow); transition:box-shadow .12s; }
.pf-kanban-card:hover { box-shadow:var(--shadow-md); }

/* Status colors */
.pf-s-new      { color:#6b7280; } .pf-sb-new      { background:#f3f4f6; color:#6b7280; }
.pf-s-planned  { color:#3b82f6; } .pf-sb-planned  { background:#dbeafe; color:#1d4ed8; }
.pf-s-inprog   { color:#8b5cf6; } .pf-sb-inprog   { background:#ede9fe; color:#7c3aed; }
.pf-s-review   { color:#f59e0b; } .pf-sb-review   { background:#fef3c7; color:#d97706; }
.pf-s-fix      { color:#ef4444; } .pf-sb-fix      { background:#fee2e2; color:#dc2626; }
.pf-s-approved { color:#10b981; } .pf-sb-approved { background:#d1fae5; color:#059669; }
.pf-s-done     { color:#16a34a; } .pf-sb-done     { background:#dcfce7; color:#15803d; }
.pf-s-hold     { color:#9ca3af; } .pf-sb-hold     { background:#f9fafb; color:#6b7280; }

/* Priority */
.pf-pri-urgent { color:#dc2626; } .pf-pri-high { color:#f59e0b; }
.pf-pri-medium { color:#3b82f6; } .pf-pri-low  { color:#9ca3af; }

/* Comment */
.pf-comment { display:flex; gap:8px; margin-bottom:12px; }
.pf-comment-av { width:30px; height:30px; border-radius:50%; background:var(--accent); color:#fff; display:flex; align-items:center; justify-content:center; font-size:12px; font-weight:700; flex-shrink:0; }
.pf-comment-bubble { background:var(--surface2); border-radius:0 10px 10px 10px; padding:8px 12px; flex:1; }
.pf-comment-meta { font-size:11px; color:var(--text3); margin-bottom:3px; display:flex; justify-content:space-between; }
.pf-comment-author { font-weight:700; color:var(--accent); }
.pf-comment-text { font-size:13px; color:var(--text1); line-height:1.5; }
.pf-comment-inp { border:1px solid var(--border); border-radius:var(--radius-sm); padding:8px 12px; width:100%; font-size:13px; font-family:var(--font); resize:none; outline:none; min-height:70px; }
.pf-comment-inp:focus { border-color:var(--accent); }


/* ══════════════════════════════════════════════
   MOBILE APP OPTIMIZATIONS FOR ANDROID APK
   ══════════════════════════════════════════════ */

/* Safe area for notch/status bar */
:root {
  --safe-top: env(safe-area-inset-top, 0px);
  --safe-bottom: env(safe-area-inset-bottom, 0px);
  --bottom-nav-h: 72px;
}

/* ── Bottom Navigation Bar ── */
.mobile-bottom-nav {
  display: none;
  position: fixed;
  bottom: 0; left: 0; right: 0;
  height: var(--bottom-nav-h);
  padding-bottom: var(--safe-bottom);
  background: var(--text1);
  border-top: 1px solid rgba(255,255,255,0.08);
  z-index: 600;
  flex-direction: row;
  align-items: stretch;
  justify-content: space-around;
}
.mbn-item {
  flex: 1;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 4px;
  cursor: pointer;
  color: rgba(255,255,255,0.45);
  font-size: 12px;
  font-weight: 700;
  position: relative;
  transition: color 0.15s;
  padding: 6px 2px;
  -webkit-tap-highlight-color: transparent;
}
.mbn-item i { font-size: 26px; }
.mbn-item.on { color: #fff; }
.mbn-item.on i { color: var(--accent-mid); }
.mbn-badge {
  position: absolute;
  top: 5px;
  left: calc(50% - 2px);
  background: var(--red);
  color: #fff;
  font-size: 8px;
  font-weight: 700;
  padding: 1px 5px;
  border-radius: 10px;
  min-width: 14px;
  text-align: center;
}
.mbn-more-btn {
  flex: 1;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 4px;
  cursor: pointer;
  color: rgba(255,255,255,0.45);
  font-size: 12px;
  font-weight: 700;
  -webkit-tap-highlight-color: transparent;
}
.mbn-more-btn i { font-size: 26px; }

/* ── More Menu Drawer ── */
.mobile-more-drawer {
  display: none;
  position: fixed;
  bottom: var(--bottom-nav-h);
  left: 0; right: 0;
  background: var(--text1);
  border-top: 1px solid rgba(255,255,255,0.1);
  border-radius: 16px 16px 0 0;
  z-index: 700;
  padding: 12px 0 8px;
  box-shadow: 0 -8px 30px rgba(0,0,0,0.3);
  transform: translateY(100%);
  transition: transform 0.25s ease;
}
.mobile-more-drawer.open {
  transform: translateY(0);
}
.mmd-item {
  display: flex;
  align-items: center;
  gap: 14px;
  padding: 16px 22px;
  color: rgba(255,255,255,0.85);
  font-size: 16px;
  cursor: pointer;
  -webkit-tap-highlight-color: transparent;
}
.mmd-item i { font-size: 24px; color: rgba(255,255,255,0.6); }
.mmd-item:active { background: rgba(255,255,255,0.06); }
.mmd-item.on { color: #fff; }
.mmd-item.on i { color: var(--accent-mid); }
.mmd-sep { height: 1px; background: rgba(255,255,255,0.07); margin: 4px 0; }
.mmd-overlay {
  display: none;
  position: fixed;
  inset: 0;
  background: rgba(0,0,0,0.4);
  z-index: 699;
}
.mmd-overlay.open { display: block; }

@media (max-width: 680px) {
  /* Show bottom nav, hide sidebar */
  .mobile-bottom-nav { display: flex !important; }
  .sidebar { display: none !important; }

  /* Adjust layout for bottom nav */
  .app { flex-direction: column; }
  .main { height: 100%; padding-bottom: var(--bottom-nav-h); }
  .content { padding: 14px; padding-bottom: calc(var(--bottom-nav-h) + 10px); }

  /* الخط العام أكبر على الموبايل */
  body { font-size: 15px !important; }
  td, th, .badge, .ec-meta-row, .rc-proj, .stat-lbl { font-size: 13px !important; }
  .stat-val { font-size: 24px !important; }
  .ec-name { font-size: 15px !important; }
  .mhd-t { font-size: 17px !important; }
  label, .fg label { font-size: 14px !important; }

  /* Topbar adjustments */
  .topbar { padding: 10px 14px; padding-top: calc(10px + var(--safe-top)); gap: 8px; flex-wrap: wrap; }
  .pg-title { font-size: 16px; font-weight: 800; }
  .gsearch { width: 100% !important; min-width: 0; }
  .search-wrap { order: 10; width: 100%; }
  .tbtn span { display: none; }
  .tbtn { padding: 8px 10px; }

  /* Stats grid: 2 cols on mobile */
  .stats-row { grid-template-columns: 1fr 1fr; gap: 10px; }
  .dash-type-grid { grid-template-columns: 1fr 1fr !important; }
  .dash-summary-grid { grid-template-columns: 1fr 1fr !important; }
  .frow { grid-template-columns: 1fr !important; }
  .frow3 { grid-template-columns: 1fr !important; }
  .fin2-kpis, .pfin-kpis { grid-template-columns: 1fr 1fr; }
  .pfin-kpis { grid-template-columns: 1fr 1fr; }
  .cards-grid { grid-template-columns: 1fr; }
  .expense-cat-grid { grid-template-columns: repeat(3, 1fr); }

  /* Modals fullscreen on mobile */
  .overlay { padding: 0; align-items: flex-end; padding-bottom: 0 !important; }
  .modal, .modal-wide { width: 100% !important; max-width: 100% !important; border-radius: 16px 16px 0 0; max-height: 90vh; overflow-y: auto; margin: 0; position: relative; z-index: 901; }
  .mhd { padding: 16px 18px 12px; }
  .mbody { padding: 16px 18px; }
  .mft { padding: 12px 18px; }

  /* Toast above bottom nav */
  .toast { bottom: calc(var(--bottom-nav-h) + 12px); right: 14px; left: 14px; text-align: center; }

  /* Tables scroll */
  .tbl-wrap { overflow-x: auto; -webkit-overflow-scrolling: touch; }
  table { min-width: 600px; }

  /* Touch-friendly tap targets */
  .tbtn, .btn-save, .btn-cancel, .lbtn { min-height: 42px; }
  .lin, .finput, .fselect, .fsel, .finp { min-height: 42px; font-size: 16px !important; }
  
  /* Prevent zoom on input focus */
  input, select, textarea { font-size: 16px !important; }

  /* Login card full-width on small screen */
  .login-card { border-radius: 0; min-height: 100vh; padding: 40px 24px; display: flex; flex-direction: column; justify-content: center; }
}

/* ── Mobile touch fixes ── */
.tbtn, .btn-save, .btn-cancel, .ni, .mbn-item, .mbn-more-btn,
.mmd-item, .icon-btn, .lbtn, button {
  -webkit-tap-highlight-color: transparent;
  touch-action: manipulation;
  cursor: pointer;
}
* { -webkit-overflow-scrolling: touch; }
</style>
</head>
<body>

<script>
// Force WebView storage to work
if (typeof Android !== 'undefined') {
  try { Android.enableLocalStorage && Android.enableLocalStorage(); } catch(e) {}
}
// Ensure window.localStorage exists
if (!window.localStorage) {
  window.localStorage = {
    _data: {},
    setItem(k,v) { this._data[k]=v; },
    getItem(k) { return this._data[k]||null; },
    removeItem(k) { delete this._data[k]; },
    clear() { this._data={}; }
  };
}
</script>

<!-- ══════════════════════════════════════════════
     MOBILE BOTTOM NAVIGATION BAR
     ══════════════════════════════════════════════ -->
<div class="mobile-bottom-nav" id="mobile-bottom-nav">
  <div class="mbn-item on" id="mbn-dashboard" onclick="sw('dashboard', document.getElementById('nav-dashboard')||this); mbnActivate('dashboard')">
    <i class="ti ti-dashboard"></i>
    <span>الرئيسية</span>
  </div>
  <div class="mbn-item" id="mbn-projects" onclick="sw('projects', document.getElementById('nav-projects')||this); mbnActivate('projects')">
    <i class="ti ti-folder-open"></i>
    <span>المشاريع</span>
  </div>
  <div class="mbn-item" id="mbn-proj-followup" onclick="sw('proj-followup', document.getElementById('nav-pf')||this); mbnActivate('proj-followup')">
    <i class="ti ti-layout-kanban"></i>
    <span>المتابعة</span>
  </div>
  <div class="mbn-item" id="mbn-finance" onclick="sw('finance', document.getElementById('nav-finance')||this); mbnActivate('finance')">
    <i class="ti ti-cash"></i>
    <span>المالية</span>
  </div>
  <div class="mbn-item" id="mbn-addtask" onclick="openWorkOrder()" style="background:var(--accent);border-radius:12px;margin:8px 4px;">
    <i class="ti ti-plus" style="font-size:28px;color:#fff;"></i>
    <span style="color:#fff;">جديد</span>
  </div>
  <div class="mbn-more-btn" onclick="toggleMoreDrawer()">
    <i class="ti ti-menu-2"></i>
    <span>المزيد</span>
  </div>
</div>

<!-- More Drawer Overlay -->
<div class="mmd-overlay" id="mmd-overlay" onclick="closeMoreDrawer()"></div>

<!-- More Drawer -->
<div class="mobile-more-drawer" id="mobile-more-drawer">
  <div class="mmd-item" id="mmd-clients" onclick="sw('clients', document.getElementById('nav-clients')||this); mbnActivate('clients'); closeMoreDrawer()">
    <i class="ti ti-users"></i> العملاء
  </div>
  <div class="mmd-item" id="mmd-eng-tasks" onclick="sw('eng-tasks', document.getElementById('nav-engtasks')||this); mbnActivate('eng-tasks'); closeMoreDrawer()">
    <i class="ti ti-checklist"></i> مهام المهندسين
  </div>
  <div class="mmd-item" id="mmd-reports" onclick="sw('reports', document.getElementById('nav-reports')||this); mbnActivate('reports'); closeMoreDrawer()">
    <i class="ti ti-report"></i> التقارير
  </div>
  <div class="mmd-sep"></div>
  <div class="mmd-item" id="mmd-settings" onclick="sw('settings', document.getElementById('nav-settings')||this); mbnActivate('settings'); closeMoreDrawer()">
    <i class="ti ti-settings"></i> الإعدادات
  </div>
  <div class="mmd-item" onclick="doLogout(); closeMoreDrawer()">
    <i class="ti ti-logout"></i> تسجيل الخروج
  </div>
</div>

<script>
// ── Mobile Bottom Nav Helpers ──
function mbnActivate(view) {
  // Bottom nav items
  document.querySelectorAll('.mbn-item').forEach(el => el.classList.remove('on'));
  const mainViews = ['dashboard', 'projects', 'proj-followup', 'finance'];
  if (mainViews.includes(view)) {
    const btn = document.getElementById('mbn-' + view);
    if (btn) btn.classList.add('on');
  }
  // More drawer items
  document.querySelectorAll('.mmd-item').forEach(el => el.classList.remove('on'));
  const mmdEl = document.getElementById('mmd-' + view);
  if (mmdEl) mmdEl.classList.add('on');
}

function toggleMoreDrawer() {
  const drawer = document.getElementById('mobile-more-drawer');
  const overlay = document.getElementById('mmd-overlay');
  const isOpen = drawer.classList.contains('open');
  if (isOpen) {
    drawer.classList.remove('open');
    overlay.classList.remove('open');
  } else {
    drawer.classList.add('open');
    overlay.classList.add('open');
  }
}

function closeMoreDrawer() {
  document.getElementById('mobile-more-drawer')?.classList.remove('open');
  document.getElementById('mmd-overlay')?.classList.remove('open');
}

// sw() patch moved to after sw() definition
</script>


<!-- ═══ LOGIN ═══════════════════════════════════════════════════════ -->
<div class="login-wrap" id="login-wrap" style="display: flex;">
  <div class="login-card">
    <div class="login-brand">
      <div class="login-mark"><i class="ti ti-building-arch"></i></div>
      <div>
        <div class="login-name">ProjexID</div>
        <div class="login-tagline">نظام إدارة المشاريع الهندسية المتكامل</div>
      </div>
    </div>
    <div class="login-fields">
      <div class="field-wrap">
        <i class="ti ti-user"></i>
        <input class="lin" id="l-user" type="text" placeholder="اسم المستخدم" autocomplete="username">
      </div>
      <div class="field-wrap">
        <i class="ti ti-lock"></i>
        <input class="lin" id="l-pass" type="password" placeholder="كلمة المرور" autocomplete="current-password" onkeydown="if(event.key==='Enter')doLogin()">
      </div>
      <div class="l-err" id="l-err"></div>
      <button class="lbtn" onclick="doLogin()">دخول <i class="ti ti-arrow-left" style="vertical-align:-2px;"></i></button>
    </div>
    <div style="margin-top:14px;padding:12px 14px;background:rgba(255,255,255,.08);border-radius:8px;font-size:11.5px;color:rgba(255,255,255,.75);line-height:2;">
    <strong style="color:#fff;">بيانات الدخول:</strong><br>
    مدير: <strong>osman</strong> / osman<br>
    مهندس: <strong>eng</strong> / eng
  </div>
  </div>
</div>

<!-- ═══ APP ═════════════════════════════════════════════════════════ -->
<div class="app" id="app" style="display: none;">

  <!-- Sidebar -->
  <aside class="sidebar">
    <div class="sb-brand">
      <div class="sb-mark"><i class="ti ti-building-arch"></i></div>
      <div>
        <div class="sb-name">ProjexID</div>
        <div class="sb-tag">Engineering PM</div>
      </div>
    </div>
    <nav class="sb-nav">
      <div class="sb-sec">الرئيسية</div>
      <div class="ni on" data-view="dashboard" onclick="sw(&#39;dashboard&#39;,this)"><i class="ti ti-dashboard"></i><span>الصفحة الرئيسية</span></div>
      <div class="sb-sec" id="sb-admin-sec">الإدارة</div>
      <div class="ni" id="nav-clients" data-view="clients" onclick="sw(&#39;clients&#39;,this)"><i class="ti ti-users"></i><span>العملاء</span></div>
      <div class="ni" id="nav-projects" data-view="projects" onclick="sw(&#39;projects&#39;,this)"><i class="ti ti-folder-open"></i><span>المشاريع</span></div>
      <div class="ni" id="nav-engtasks" data-view="eng-tasks" onclick="sw(&#39;eng-tasks&#39;,this)"><i class="ti ti-checklist"></i><span>مهام المهندسين</span><span class="nbadge" id="badge-tasks" style="display: none;"></span></div>
      <div class="ni" id="nav-pf" data-view="proj-followup" onclick="sw(&#39;proj-followup&#39;,this)"><i class="ti ti-layout-kanban"></i><span>متابعة المشاريع</span></div>
      <div class="sb-sec" id="sb-finance-sec">المالية والتقارير</div>
      <div class="ni" id="nav-finance" data-view="finance" onclick="sw(&#39;finance&#39;,this)" style="display: flex;"><i class="ti ti-cash"></i><span>الشؤون المالية</span></div>
      <div class="ni" id="nav-reports" data-view="reports" onclick="sw(&#39;reports&#39;,this)"><i class="ti ti-report"></i><span>التقارير</span></div>
      <div class="sb-sec" id="sb-system-sec">النظام</div>
      <div class="ni" id="nav-settings" data-view="settings" onclick="sw(&#39;settings&#39;,this)"><i class="ti ti-settings"></i><span>الإعدادات</span></div>
      <div class="ni" onclick="doLogout()"><i class="ti ti-logout"></i><span>تسجيل الخروج</span></div>
    </nav>
    <div class="sb-user">
      <div class="av" style="width:34px;height:34px;background:var(--accent);" id="u-av">أ</div>
      <div class="user-info" style="flex:1;min-width:0;">
        <div style="font-size:12.5px;font-weight:700;color:rgba(255,255,255,0.9);" id="u-name">أسمان</div>
        <div style="font-size:10px;color:rgba(255,255,255,0.4);" id="u-role">مدير المشاريع</div>
      </div>
    </div>
  </aside>

  <!-- Main -->
  <main class="main">
    <div class="topbar">
      <div class="pg-title" id="pg-title">الصفحة الرئيسية</div>
      <div class="search-wrap">
        <i class="ti ti-search"></i>
        <input class="gsearch" id="gsearch" placeholder="بحث عالمي..." oninput="globalSearch()">
      </div>
      <button class="tbtn pr" id="btn-add-task" onclick="openWorkOrder()" style="display: flex; position:relative; z-index:10;"><i class="ti ti-plus"></i> أمر عمل جديد</button>
      <button class="tbtn pr" id="btn-add-client" onclick="openAddClient()" style="display:none;"><i class="ti ti-user-plus"></i> إضافة عميل</button>
      <button class="tbtn pr" id="btn-add-report" onclick="openReportModal()" style="display:none;"><i class="ti ti-plus"></i> تقرير جديد</button>
    </div>

    <div class="content">

      <!-- ══ DASHBOARD ══════════════════════════════════════════════ -->
      <div class="view on" id="view-dashboard">
        <div class="stats-row" id="dash-stats">
    <div class="stat-card sc-blue">
      <div class="stat-icon" style="background:var(--blue-light);">
        <i class="ti ti-users" style="color:var(--blue);"></i>
        <span class="stat-icon-label" style="color:var(--blue);">إجمالي العملاء</span>
      </div>
      <div class="stat-val">0</div>
      <div class="stat-sub" style="color:var(--blue);">0 مشروع مرتبط</div>
    </div>
    <div class="stat-card sc-green">
      <div class="stat-icon" style="background:var(--green-light);">
        <i class="ti ti-folder-open" style="color:var(--green);"></i>
        <span class="stat-icon-label" style="color:var(--green);">إجمالي المشاريع</span>
      </div>
      <div class="stat-val">0</div>
      <div class="stat-sub" style="color:var(--green);">0 نشط</div>
    </div>
    <div class="stat-card sc-amber">
      <div class="stat-icon" style="background:var(--amber-light);">
        <i class="ti ti-check" style="color:var(--amber);"></i>
        <span class="stat-icon-label" style="color:var(--amber);">مشاريع مكتملة</span>
      </div>
      <div class="stat-val">0</div>
      <div class="stat-sub" style="color:var(--amber);">0% من الإجمالي</div>
    </div>
    <div class="stat-card sc-red">
      <div class="stat-icon" style="background:var(--red-light);">
        <i class="ti ti-alert-triangle" style="color:var(--red);"></i>
        <span class="stat-icon-label" style="color:var(--red);">متأخرة التسليم</span>
      </div>
      <div class="stat-val">0</div>
      <div class="stat-sub" style="color:var(--red);">لا تأخيرات!</div>
    </div></div>
        <div style="display:flex;flex-direction:column;gap:18px;margin-bottom:20px;">
          <div>
            <div class="sec-hd">المشاريع حسب النوع <span class="sec-hd-link" onclick="sw(&#39;projects&#39;,document.querySelector(&#39;[data-view=projects]&#39;))">عرض الكل</span></div>
            <div class="card" style="padding:16px;" id="dash-type-chart"><div style="display:flex;align-items:center;gap:10px;margin-bottom:10px;">
      <span style="width:22px;font-size:16px;">🎨</span>
      <span style="font-size:12px;min-width:100px;color:var(--text2);">تصميم</span>
      <div class="prog-bar" style="flex:1;height:8px;"><div class="prog-fill" style="width:0%;"></div></div>
      <span style="font-size:12px;font-weight:600;min-width:30px;text-align:left;">0</span>
    </div><div style="display:flex;align-items:center;gap:10px;margin-bottom:10px;">
      <span style="width:22px;font-size:16px;">📋</span>
      <span style="font-size:12px;min-width:100px;color:var(--text2);">رخصة بناء</span>
      <div class="prog-bar" style="flex:1;height:8px;"><div class="prog-fill" style="width:0%;"></div></div>
      <span style="font-size:12px;font-weight:600;min-width:30px;text-align:left;">0</span>
    </div><div style="display:flex;align-items:center;gap:10px;margin-bottom:10px;">
      <span style="width:22px;font-size:16px;">👁️</span>
      <span style="font-size:12px;min-width:100px;color:var(--text2);">إشراف</span>
      <div class="prog-bar" style="flex:1;height:8px;"><div class="prog-fill" style="width:0%;"></div></div>
      <span style="font-size:12px;font-weight:600;min-width:30px;text-align:left;">0</span>
    </div><div style="display:flex;align-items:center;gap:10px;margin-bottom:10px;">
      <span style="width:22px;font-size:16px;">🔨</span>
      <span style="font-size:12px;min-width:100px;color:var(--text2);">تنفيذ</span>
      <div class="prog-bar" style="flex:1;height:8px;"><div class="prog-fill" style="width:0%;"></div></div>
      <span style="font-size:12px;font-weight:600;min-width:30px;text-align:left;">0</span>
    </div><div style="display:flex;align-items:center;gap:10px;margin-bottom:10px;">
      <span style="width:22px;font-size:16px;">📊</span>
      <span style="font-size:12px;min-width:100px;color:var(--text2);">إدارية</span>
      <div class="prog-bar" style="flex:1;height:8px;"><div class="prog-fill" style="width:0%;"></div></div>
      <span style="font-size:12px;font-weight:600;min-width:30px;text-align:left;">0</span>
    </div></div>
          </div>
          <div>
            <div class="sec-hd">آخر النشاطات</div>
            <div class="card" style="padding:0;" id="dash-activity"><div class="empty"><i class="ti ti-clock"></i><p>لا نشاطات</p></div></div>
          </div>
        </div>
        <div class="sec-hd">آخر المشاريع المضافة <span class="sec-hd-link" onclick="sw(&#39;projects&#39;,document.querySelector(&#39;[data-view=projects]&#39;))">عرض الكل</span></div>
        <div class="card tbl-wrap"><table id="dash-recent-tbl"><tbody><tr><td colspan="6" style="text-align:center;color:var(--text3);padding:30px;">لا توجد مشاريع</td></tr></tbody></table></div>
      </div>

      <!-- ══ CLIENTS ════════════════════════════════════════════════ -->
      <div class="view" id="view-clients">
        <div class="filter-bar">
          <input class="finput" id="client-search" placeholder="🔍 ابحث عن عميل..." oninput="renderClients()">
          <button class="tbtn pr" id="clients-add-btn" onclick="openAddClient()" style="display:none;"><i class="ti ti-user-plus"></i> إضافة عميل</button>
        </div>
        <div class="cards-grid" id="clients-grid"><div class="empty" style="grid-column:1/-1;"><i class="ti ti-users"></i><p>لا يوجد عملاء</p></div></div>
      </div>

      <!-- ══ PROJECTS ═══════════════════════════════════════════════ -->
      <div class="view" id="view-projects">
        <div class="filter-bar">
          <input class="finput" id="proj-search" placeholder="🔍 ابحث عن مشروع..." oninput="renderProjects()">
          <select class="fselect" id="proj-filter-type" onchange="renderProjects()">
            <option value="">كل الأنواع</option>
            <option value="design">تصميم</option>
            <option value="permit">رخصة بناء</option>
            <option value="super">إشراف</option>
            <option value="exec">تنفيذ</option>
            <option value="admin">إدارية</option>
          </select>
          <select class="fselect" id="proj-filter-status" onchange="renderProjects()">
            <option value="">كل الحالات</option>
            <option value="waiting">قائمة الانتظار</option>
            <option value="inprog">قيد التنفيذ</option>
            <option value="review">قيد المراجعة</option>
            <option value="done">مكتمل</option>
            <option value="hold">متوقف</option>
            <option value="waitclient">انتظار العميل</option>
          </select>
          <select class="fselect" id="proj-filter-eng" onchange="renderProjects()">
            <option value="">كل المهندسين</option>
          <option value="1001">أحمد الرشيدي</option><option value="1002">سارة المحمود</option><option value="1003">نور الحسيني</option></select>
        </div>
        <div class="card tbl-wrap"><table id="projects-tbl"><thead><tr>
          <th>رقم المشروع</th><th>العميل</th><th>النوع</th><th>الوصف</th><th>المهندس</th><th>الأولوية</th><th>الحالة</th><th>التسليم</th><th>الإنجاز</th><th></th>
        </tr></thead><tbody id="projects-tbody"><tr><td colspan="10" style="text-align:center;color:var(--text3);padding:30px;">لا توجد مشاريع مطابقة</td></tr></tbody></table></div>
      </div>

      <!-- ══ ENGINEER TASKS ═════════════════════════════════════════ -->
      <div class="view" id="view-eng-tasks">
        <!-- View toggle -->
        <div style="margin-bottom:10px;display:flex;align-items:center;gap:10px;flex-wrap:wrap;">
          <div class="et-view-toggle">
            <button class="et-view-btn on" id="et-vbtn-normal"   onclick="setEtView('normal')">
              <i class="ti ti-layout-list"></i> عرض عادي
            </button>
            <button class="et-view-btn"    id="et-vbtn-byengineer" onclick="setEtView('byengineer')">
              <i class="ti ti-users"></i> حسب المهندس
            </button>
          </div>
        </div>
        <div class="filter-bar" id="et-filter-bar">
          <select class="fselect" id="et-filter-status" onchange="renderEngTasks()">
            <option value="">كل الحالات</option>
            <option value="waiting">قائمة الانتظار</option>
            <option value="inprog">قيد التنفيذ</option>
            <option value="review">قيد المراجعة</option>
            <option value="done">مكتمل</option>
            <option value="hold">متوقف</option>
            <option value="waitclient">انتظار العميل</option>
          </select>
          <select class="fselect" id="et-filter-pri" onchange="renderEngTasks()">
            <option value="">كل الأولويات</option>
            <option value="urgent">عاجل</option>
            <option value="medium">متوسط</option>
            <option value="low">منخفض</option>
          </select>
        </div>
        <div id="eng-tasks-list"></div>
        <div id="eng-tasks-byeng" style="display:none;"></div>
      </div>

      <!-- ══ FINANCE ════════════════════════════════════════════════ -->
      <div class="view" id="view-finance">
        <!-- Global KPI Hero -->
        <div class="fin2-hero">
          <div class="fin2-hero-top">
            <div>
              <div class="fin2-hero-title"><i class="ti ti-building-bank" style="vertical-align:-3px;margin-left:8px;"></i>الإدارة المالية</div>
              <div class="fin2-hero-sub">ملخص شامل لجميع المشاريع والعملاء</div>
            </div>
            <div style="display:flex;gap:8px;flex-wrap:wrap;">
              <button class="pfin-btn pfin-btn-print" onclick="printGlobalStatement()"><i class="ti ti-printer"></i> كشف شامل</button>
              <button class="pfin-btn pfin-btn-export" onclick="exportGlobalFinance()"><i class="ti ti-file-spreadsheet"></i> تصدير Excel</button>
            </div>
          </div>
          <div class="fin2-kpis" id="fin2-global-kpis">
            <div class="fin2-kpi"><div class="fin2-kpi-lbl">قيمة العقود</div><div class="fin2-kpi-val">—</div></div>
            <div class="fin2-kpi pos"><div class="fin2-kpi-lbl">إجمالي المحصّل</div><div class="fin2-kpi-val">—</div></div>
            <div class="fin2-kpi warn"><div class="fin2-kpi-lbl">إجمالي المصروفات</div><div class="fin2-kpi-val">—</div></div>
            <div class="fin2-kpi neg"><div class="fin2-kpi-lbl">المتبقي على العملاء</div><div class="fin2-kpi-val">—</div></div>
            <div class="fin2-kpi pos"><div class="fin2-kpi-lbl">صافي الربح</div><div class="fin2-kpi-val">—</div></div>
          </div>
        </div>
        <!-- Section tabs -->
        <div class="filter-bar" style="margin-bottom:16px;flex-wrap:wrap;gap:10px;">
          <div class="fin-sec-tabs">
            <button class="fin-sec-tab on" id="fin-tab-clients"
              onclick="setFinTab('clients')"><i class="ti ti-users"></i>العملاء</button>
            <button class="fin-sec-tab" id="fin-tab-ws"
              onclick="setFinTab('ws')"><i class="ti ti-building-warehouse"></i>حساب الورشات</button>
            <button class="fin-sec-tab" id="fin-tab-wk"
              onclick="setFinTab('wk')"><i class="ti ti-hard-hat"></i>حساب العمال</button>
          </div>
          <!-- Back + Summary buttons (shown only when NOT on clients tab) -->
          <button class="tbtn" id="fin-back-btn" onclick="setFinTab('clients')"
            style="display:none;"><i class="ti ti-arrow-right"></i> رجوع للعملاء</button>
          <button class="pfin-btn pfin-btn-print" id="fin-ws-summary-btn"
            onclick="printWorkshopSummary()" style="display:none;">
            <i class="ti ti-file-text"></i> ملخص مالي شامل
          </button>
          <input class="finput" id="fin2-search"
            placeholder="🔍 بحث..." oninput="renderFinance()" style="min-width:180px;">
          <select class="fselect" id="fin2-filter-status" onchange="renderFinance()">
            <option value="">كل المشاريع</option>
            <option value="has_debt">عليه متبقي</option>
            <option value="paid">مسدد بالكامل</option>
            <option value="has_expenses">لديه مصروفات</option>
          </select>
        </div>
        <!-- Client cards (default) -->
        <div class="cards-grid" id="finance-grid">
          <div class="empty" style="grid-column:1/-1;"><i class="ti ti-cash"></i><p>لا يوجد عملاء بعد</p></div>
        </div>
        <!-- Workshops financial cards -->
        <div id="fin-ws-grid" style="display:none;"></div>
        <!-- Workers financial cards -->
        <div id="fin-wk-grid" style="display:none;"></div>
        <!-- Daily site log reports -->
        <div class="dash-daily-strip">
          <div class="dash-daily-title">
            <i class="ti ti-clipboard-list" style="font-size:18px;color:var(--accent);"></i>
            آخر التقارير اليومية للموقع
            <button class="tbtn" onclick="sw('reports',document.querySelector('[data-view=reports]'))" style="font-size:11px;padding:5px 12px;margin-right:auto;">
              كل التقارير <i class="ti ti-arrow-left"></i>
            </button>
          </div>
          <div style="display:flex;flex-direction:column;gap:8px;" id="dash-daily-reports">
            <div style="color:var(--text3);font-size:12px;padding:8px 0;">—</div>
          </div>
        </div>
      </div>

      <!-- ══ REPORTS ════════════════════════════════════════════════ -->
      <div class="view" id="view-reports">
        <!-- Stats banner -->
        <div id="rep-hero-banner"></div>
        <!-- Group toggle + Filters -->
        <div style="margin-bottom:10px;display:flex;align-items:center;gap:10px;flex-wrap:wrap;">
          <button class="tbtn" id="rep-back-btn" onclick="setRepGroup('none')" style="display:none;"><i class="ti ti-arrow-right"></i> رجوع للعرض العادي</button>
          <div class="rep-group-toggle" id="rep-group-toggle">
            <button class="rep-group-btn on" id="rg-none"    onclick="setRepGroup('none')">☰ عادي</button>
            <button class="rep-group-btn"    id="rg-project" onclick="setRepGroup('project')">📁 حسب المشروع</button>
            <button class="rep-group-btn"    id="rg-client"  onclick="setRepGroup('client')">👤 حسب العميل</button>
            <button class="rep-group-btn"    id="rg-engineer"onclick="setRepGroup('engineer')">👷 حسب المهندس</button>
          </div>
        </div>
        <div class="filter-bar" style="flex-wrap:wrap;gap:8px;" id="rep-filter-bar">
          <select class="fselect" id="rep-filter-type" onchange="renderReports()">
            <option value="">كل التقارير</option>
            <option value="daily_site">📅 سجل يومي للموقع</option>
            <option value="daily">📅 يومي</option>
            <option value="weekly">📊 أسبوعي</option>
            <option value="milestone">🏁 مرحلي</option>
            <option value="final">✅ نهائي</option>
          </select>
          <select class="fselect" id="rep-filter-proj" onchange="renderReports()">
            <option value="">كل المشاريع</option>
          </select>
          <select class="fselect" id="rep-filter-eng" onchange="renderReports()">
            <option value="">كل المهندسين</option>
          </select>
          <select class="fselect" id="rep-filter-ws" onchange="renderReports()">
            <option value="">كل الورشات</option>
          </select>
          <input class="finput" type="date" id="rep-filter-from"
            placeholder="من تاريخ" onchange="renderReports()" title="من تاريخ" style="width:140px;">
          <input class="finput" type="date" id="rep-filter-to"
            placeholder="إلى تاريخ" onchange="renderReports()" title="إلى تاريخ" style="width:140px;">
          <select class="fselect" id="rep-sort" onchange="renderReports()">
            <option value="newest">الأحدث أولًا</option>
            <option value="oldest">الأقدم أولًا</option>
            <option value="project">حسب المشروع</option>
            <option value="workshop">حسب الورشة</option>
            <option value="engineer">حسب المهندس</option>
          </select>
        </div>
        <!-- All projects list (shown before filtering) -->
        <div id="rep-all-projects" style="margin:12px 0 16px;"></div>
        <div style="display:grid;grid-template-columns:repeat(auto-fill,minmax(300px,1fr));gap:14px;" id="reports-grid">
          <div class="empty" style="grid-column:1/-1;"><i class="ti ti-report"></i><p>لا توجد تقارير</p></div>
        </div>
      </div>

      <!-- ══ SETTINGS ═══════════════════════════════════════════════ -->
      <div class="view" id="view-settings">
        <div class="settings-layout">
          <!-- Side nav -->
          <div class="settings-sidenav">
            <div class="set-nav-item on" id="snav-company"  onclick="setTab('company')"><i class="ti ti-building"></i>الشركة</div>
            <div class="set-nav-item"    id="snav-users"    onclick="setTab('users')"><i class="ti ti-users-group"></i>المستخدمون</div>
            <div class="set-nav-item"    id="snav-finance"  onclick="setTab('finance')"><i class="ti ti-coin"></i>الشؤون المالية</div>
            <div class="set-nav-item"    id="snav-reports"  onclick="setTab('reports')"><i class="ti ti-report"></i>التقارير</div>
            <div class="set-nav-item"    id="snav-projects" onclick="setTab('projects')"><i class="ti ti-folder"></i>المشاريع</div>
            <div class="set-nav-item"    id="snav-security" onclick="setTab('security')"><i class="ti ti-lock"></i>الأمان</div>
            <div class="set-nav-item"    id="snav-data"     onclick="setTab('data')"><i class="ti ti-database"></i>البيانات</div>
            <div class="set-nav-item"    id="snav-log"      onclick="setTab('log')"><i class="ti ti-history"></i>سجل النشاط</div>
          </div>
          <!-- Content -->
          <div id="set-content"></div>
        </div>

<!-- ══ PROJECT FOLLOWUP ══════════════════════════════════════════ -->
<div class="view" id="view-proj-followup">
  <div class="pf-layout">
    <!-- Left: project list -->
    <div class="pf-proj-list">
      <div class="pf-proj-search">
        <input id="pf-search" placeholder="🔍 بحث عن مشروع..." oninput="renderProjFollowup()">
      </div>
      <div id="pf-proj-items"></div>
    </div>
    <!-- Right: stages + tasks -->
    <div class="pf-main" id="pf-main">
      <div class="empty" style="margin:auto;">
        <i class="ti ti-layout-kanban" style="font-size:40px;color:var(--border2);"></i>
        <p>اختر مشروعاً من القائمة</p>
      </div>
    </div>
  </div>
</div>

      </div>

    </div>
  </main>
</div>

<!-- ══════════════════════════════════════════════════════════════════
     WORK ORDER MODAL (3 Cards)
═══════════════════════════════════════════════════════════════════ -->
<div class="overlay" id="wo-overlay" onclick="if(event.target===this)closeWO()">
  <div class="modal modal-wide" onclick="event.stopPropagation()">
    <div class="mhd">
      <div>
        <div class="mhd-t" id="wo-title">أمر عمل جديد</div>
        <div class="mhd-sub">أدخل بيانات المشروع في الأقسام الثلاثة</div>
      </div>
      <button class="icon-btn" onclick="closeWO()" style="display:flex;align-items:center;gap:4px;padding:5px 10px;border-radius:6px;"><i class="ti ti-x"></i> إغلاق</button>
    </div>
    <div class="mbody">

      <!-- Card 1: Client -->
      <div class="sec-card client-card">
        <div class="sec-card-header">
          <div class="sec-card-icon"><i class="ti ti-users"></i></div>
          <div>
            <div class="sec-card-title">القسم الأول — العميل</div>
            <div style="font-size:11px;color:var(--client-c);opacity:0.8;">بيانات صاحب المشروع</div>
          </div>
        </div>
        <div class="frow">
          <div class="fg">
            <label>العميل <span class="req">*</span></label>
            <select class="fi" id="wo-client" onchange="onClientChange()"><option value="">اختر عميلاً...</option><option value="NEW">+ عميل جديد</option></select>
          </div>
          <div class="fg">
            <label>رقم العميل</label>
            <input class="fi" id="wo-client-code" readonly="" placeholder="تلقائي">
          </div>
        </div>
        <div id="new-client-fields" style="display:none;">
          <div class="frow" style="margin-bottom:10px;">
            <div class="fg">
              <label>اسم العميل الجديد <span class="req">*</span></label>
              <input class="fi" id="wo-new-client-name" placeholder="اسم العميل...">
            </div>
            <div class="fg">
              <label>رقم الهاتف <span class="req">*</span></label>
              <input class="fi" id="wo-new-client-phone" placeholder="+9665...">
            </div>
          </div>
          <div class="fg">
            <label>البريد الإلكتروني</label>
            <input class="fi" id="wo-new-client-email" type="email" placeholder="(اختياري)">
          </div>
        </div>
      </div>

      <!-- Card 2: Project -->
      <div class="sec-card project-card">
        <div class="sec-card-header">
          <div class="sec-card-icon"><i class="ti ti-folder-open"></i></div>
          <div>
            <div class="sec-card-title">القسم الثاني — المشروع</div>
            <div style="font-size:11px;color:var(--project-c);opacity:0.8;">تفاصيل العمل الهندسي</div>
          </div>
        </div>
        <div class="frow">
          <div class="fg">
            <label>نوع المشروع <span class="req">*</span></label>
            <select class="fi" id="wo-type" onchange="onTypeChange()">
              <option value="design">🎨 تصميم</option>
              <option value="permit">📋 رخصة بناء</option>
              <option value="super">👁️ إشراف</option>
              <option value="exec">🔨 تنفيذ</option>
              <option value="admin">📊 أمور إدارية</option>
            </select>
          </div>
          <div class="fg">
            <label>رقم المشروع</label>
            <input class="fi" id="wo-proj-code" readonly="" placeholder="تلقائي">
          </div>
        </div>
        <div class="fg">
          <label>وصف العمل</label>
          <textarea class="fi" id="wo-desc" placeholder="اكتب وصفاً تفصيلياً للمهام المطلوبة..."></textarea>
        </div>
        <div class="frow">
          <div class="fg">
            <label>رقم العقار</label>
            <input class="fi" id="wo-prop-num" placeholder="(اختياري)">
          </div>
          <div class="fg">
            <label>الحي / المنطقة</label>
            <input class="fi" id="wo-district" placeholder="(اختياري)">
          </div>
        </div>
        <!-- Attachments -->
        <div class="fg">
          <label>المرفقات</label>
          <div class="file-drop" onclick="document.getElementById(&#39;wo-files-inp&#39;).click()">
            <i class="ti ti-cloud-upload"></i>
            <span>اضغط لرفع ملفات (JPG، PDF، DWG، ZIP...)</span>
          </div>
          <input type="file" id="wo-files-inp" multiple="" accept=".jpg,.jpeg,.png,.webp,.pdf,.docx,.xlsx,.dwg,.dxf,.zip,.rar,.ifc" style="display:none;" onchange="onFilesSelected()">
          <div class="file-list" id="wo-file-list"></div>
        </div>
        <!-- Financial -->
        <div style="border-top:1px solid rgba(0,0,0,0.10);padding-top:14px;margin-top:2px;">
          <div style="font-size:12px;font-weight:700;color:var(--project-c);margin-bottom:10px;"><i class="ti ti-coin" style="vertical-align:-2px;margin-left:5px;"></i>البنية المالية</div>
          <div class="fg">
            <label>قيمة العقد المتفق عليها</label>
            <div style="display:flex;gap:8px;align-items:center;">
              <input class="fi" type="number" id="wo-total" placeholder="0" min="0" style="flex:1;">
              <select class="fi" id="wo-currency" style="width:160px;">
                <option value="USD">$ دولار</option>
                <option value="SYP">ل.س ليرة سورية</option>
              </select>
            </div>
          </div>
        </div>
      </div>

      <!-- Card 3: Execution -->
      <div class="sec-card exec-card">
        <div class="sec-card-header">
          <div class="sec-card-icon"><i class="ti ti-settings-cog"></i></div>
          <div>
            <div class="sec-card-title">القسم الثالث — التنفيذ</div>
            <div style="font-size:11px;color:var(--exec-c);opacity:0.8;">الجدولة والمتابعة</div>
          </div>
        </div>
        <div class="frow">
          <div class="fg">
            <label>الأولوية</label>
            <select class="fi" id="wo-pri">
              <option value="urgent">🔴 عاجل</option>
              <option value="medium" selected="">🟡 متوسط</option>
              <option value="low">🟢 منخفض</option>
            </select>
          </div>
          <div class="fg">
            <label>تاريخ الاستلام</label>
            <input class="fi" id="wo-recv-date" readonly="">
          </div>
        </div>
        <div class="frow">
          <div class="fg">
            <label>تاريخ التسليم</label>
            <input class="fi" type="date" id="wo-del-date">
          </div>
          <div class="fg">
            <label>المهندس المسؤول</label>
            <input class="fi" list="wo-engineer-list" id="wo-engineer-name" placeholder="اختر مهندساً أو اكتب اسماً جديداً" oninput="onEngineerNameChange()">
            <datalist id="wo-engineer-list"></datalist>
            <input type="hidden" id="wo-engineer-id" value="">
          </div>
        </div>
        <div class="fg">
          <label>رقم واتساب المهندس</label>
          <input class="fi" id="wo-eng-wa" readonly="" placeholder="يُملأ تلقائياً">
        </div>
        <div class="frow">
          <div class="fg">
            <label>الحالة</label>
            <select class="fi" id="wo-status">
              <option value="waiting">قائمة الانتظار</option>
              <option value="inprog">قيد التنفيذ</option>
              <option value="review">قيد المراجعة</option>
              <option value="done">مكتمل</option>
              <option value="hold">متوقف</option>
              <option value="waitclient">انتظار العميل</option>
            </select>
          </div>
        </div>
      </div>
    </div>
    <div class="mft">
      <button class="btn-cancel" onclick="closeWO()">إلغاء</button>
      <button class="btn-save" onclick="saveWO()"><i class="ti ti-device-floppy" style="vertical-align:-2px;margin-left:5px;"></i> حفظ أمر العمل</button>
    </div>
  </div>
</div>

<!-- ══ ENGINEER UPDATE MODAL ════════════════════════════════════════ -->
<div class="overlay" id="eng-upd-overlay" onclick="if(event.target===this)closeEngUpd()">
  <div class="modal" onclick="event.stopPropagation()">
    <div class="mhd">
      <div><div class="mhd-t">تحديث المهمة</div><div class="mhd-sub" id="eu-subtitle"></div></div>
      <button class="icon-btn" onclick="closeEngUpd()" style="display:flex;align-items:center;gap:4px;padding:5px 10px;border-radius:6px;"><i class="ti ti-x"></i> إغلاق</button>
    </div>
    <div class="mbody">
      <div class="frow">
        <div class="fg">
          <label>الحالة</label>
          <select class="fi" id="eu-status">
            <option value="waiting">قائمة الانتظار</option>
            <option value="inprog">قيد التنفيذ</option>
            <option value="review">قيد المراجعة</option>
            <option value="done">مكتمل</option>
            <option value="hold">متوقف</option>
            <option value="waitclient">انتظار العميل</option>
          </select>
        </div>
        <div class="fg">
          <label>نسبة الإنجاز (%)</label>
          <input class="fi" type="number" id="eu-progress" min="0" max="100">
        </div>
      </div>
      <div class="fg">
        <label>ملاحظات المهندس</label>
        <textarea class="fi" id="eu-notes" placeholder="أضف ملاحظاتك..."></textarea>
      </div>
    </div>
    <div class="mft">
      <button class="btn-cancel" onclick="closeEngUpd()">إلغاء</button>
      <button class="btn-save" onclick="saveEngUpd()">حفظ التحديث</button>
    </div>
  </div>
</div>

<!-- ══ REPORT MODAL ══════════════════════════════════════════════════ -->
<div class="overlay" id="rep-overlay" onclick="if(event.target===this)closeRepModal()">
  <div class="modal modal-wide" onclick="event.stopPropagation()">
    <div class="mhd">
      <div>
        <div class="mhd-t">📋 تقرير جديد</div>
        <div class="mhd-sub" id="rep-num-preview" style="font-family:monospace;color:var(--accent);">رقم التقرير: —</div>
      </div>
      <button class="icon-btn" onclick="closeRepModal()" style="display:flex;align-items:center;gap:4px;padding:5px 10px;border-radius:6px;"><i class="ti ti-x"></i> إغلاق</button>
    </div>
    <div class="mbody">

      <!-- Row 1: Project + Type -->
      <div class="frow">
        <div class="fg">
          <label>المشروع <span class="req">*</span></label>
          <select class="fi" id="rep-project" onchange="onRepProjChange()">
            <option value="">اختر مشروعاً...</option>
          </select>
        </div>
        <div class="fg">
          <label>نوع التقرير <span class="req">*</span></label>
          <select class="fi" id="rep-type">
            <option value="daily">📅 يومي</option>
            <option value="weekly">📊 أسبوعي</option>
            <option value="milestone">🏁 مرحلي</option>
            <option value="final">✅ نهائي</option>
          </select>
        </div>
      </div>

      <!-- Project summary (injected after selection) -->
      <div id="rep-proj-info" style="display:none;">
        <div class="eu-proj-banner" id="rep-proj-banner"></div>
      </div>

      <!-- Row 2: Engineer (readonly) + Date -->
      <div class="frow">
        <div class="fg">
          <label>المهندس</label>
          <input class="fi" id="rep-engineer-display" readonly placeholder="تلقائي من الجلسة">
        </div>
        <div class="fg">
          <label>تاريخ التقرير</label>
          <input class="fi" type="date" id="rep-date">
        </div>
      </div>

      <!-- Progress snapshot -->
      <div class="fg">
        <label>لقطة نسبة الإنجاز: <strong id="rep-prog-display" style="color:var(--accent);">0</strong>%</label>
        <div class="rep-prog-display">
          <input class="eu-prog-slider" type="range" id="rep-progress" min="0" max="100" value="0"
            oninput="document.getElementById('rep-prog-display').textContent=this.value;document.getElementById('rep-prog-fill').style.width=this.value+'%'">
          <div class="prog-bar" style="flex:1;height:8px;">
            <div class="prog-fill" id="rep-prog-fill" style="width:0%;"></div>
          </div>
          <span class="rep-prog-pct-badge" id="rep-prog-pct-badge">0%</span>
        </div>
      </div>

      <!-- Content -->
      <div class="fg">
        <label>محتوى التقرير <span class="req">*</span></label>
        <textarea class="fi" id="rep-content"
          placeholder="اكتب تفاصيل ما تم إنجازه في هذه الفترة..."
          style="min-height:110px;"
          oninput="updateRepCharCount(this)"></textarea>
        <div style="font-size:10px;color:var(--text3);text-align:left;margin-top:2px;" id="rep-char-count">0 حرف</div>
      </div>

      <!-- Stages -->
      <div class="fg">
        <label>مراحل وبنود العمل المنجزة</label>
        <textarea class="fi" id="rep-stages"
          placeholder="• المرحلة الأولى: ...&#10;• المرحلة الثانية: ..."
          style="min-height:80px;"></textarea>
      </div>

      <!-- Notes -->
      <div class="fg">
        <label>ملاحظات وتوصيات</label>
        <textarea class="fi" id="rep-notes"
          placeholder="أي ملاحظات، مشاكل واجهتها، أو توصيات للمرحلة القادمة..."
          style="min-height:70px;"></textarea>
      </div>

      <!-- File Attachments -->
      <div class="fg">
        <label><i class="ti ti-paperclip" style="vertical-align:-2px;margin-left:4px;"></i>المرفقات</label>
        <div class="rep-file-drop" onclick="document.getElementById('rep-files-inp').click()">
          <i class="ti ti-cloud-upload"></i>
          <span>اضغط لرفع صور، مستندات، أو ملفات (JPG، PDF، DWG، DOCX، ZIP...)</span>
        </div>
        <input type="file" id="rep-files-inp" multiple
          accept=".jpg,.jpeg,.png,.webp,.gif,.pdf,.docx,.xlsx,.dwg,.dxf,.zip,.rar,.ifc,.mp4,.mov"
          style="display:none;" onchange="onRepFilesSelected()">
        <div class="rep-form-preview" id="rep-file-preview"></div>
      </div>

    </div>
    <div class="mft">
      <div style="font-size:11px;color:var(--text3);" id="rep-save-hint">سيتم حفظ التقرير مع جميع المرفقات</div>
      <div style="display:flex;gap:10px;">
        <button class="btn-cancel" onclick="closeRepModal()">إلغاء</button>
        <button class="btn-save" onclick="saveReport()" id="rep-save-btn">
          <i class="ti ti-device-floppy" style="vertical-align:-2px;margin-left:4px;"></i> حفظ التقرير
        </button>
      </div>
    </div>
  </div>
</div>

<!-- ══ REPORT DETAIL MODAL ════════════════════════════════════════ -->
<div class="overlay" id="rep-detail-overlay" onclick="if(event.target===this)closeRepDetail()">
  <div class="modal modal-wide" onclick="event.stopPropagation()" id="rep-detail-modal">
    <div class="mhd">
      <div>
        <div class="mhd-t" id="rd-title">تفاصيل التقرير</div>
        <div class="mhd-sub" id="rd-subtitle"></div>
      </div>
      <div style="display:flex;gap:8px;align-items:center;">
        <button class="tbtn" onclick="printReport()" id="rd-print-btn"><i class="ti ti-printer"></i> طباعة</button>
        <button class="icon-btn del" onclick="deleteReportConfirm()" id="rd-delete-btn" style="display:none;" title="حذف التقرير"><i class="ti ti-trash"></i> حذف</button>
        <button class="icon-btn" onclick="closeRepDetail()" style="display:flex;align-items:center;gap:4px;padding:5px 10px;border-radius:6px;"><i class="ti ti-x"></i> إغلاق</button>
      </div>
    </div>
    <div class="mbody" id="rd-body" style="gap:14px;"></div>
    <div class="mft">
      <button class="btn-cancel" onclick="closeRepDetail()">إغلاق</button>
    </div>
  </div>
</div>

<!-- ══ PROJECT FINANCE MODAL ═════════════════════════════════════════ -->
<div class="overlay" id="pfin-overlay" onclick="if(event.target===this)closeProjFin()">
  <div class="modal modal-wide" onclick="event.stopPropagation()" style="max-height:90vh;display:flex;flex-direction:column;">
    <div class="mhd" style="flex-shrink:0;">
      <div>
        <div class="mhd-t" id="pfin-title">المالية — المشروع</div>
        <div class="mhd-sub" id="pfin-sub"></div>
      </div>
      <button class="icon-btn" onclick="closeProjFin()" style="display:flex;align-items:center;gap:4px;padding:5px 10px;border-radius:6px;"><i class="ti ti-x"></i> إغلاق</button>
    </div>
    <!-- KPI strip -->
    <div class="pfin-kpis" id="pfin-kpis" style="flex-shrink:0;"></div>
    <!-- Workforce cards (exec/super only — populated by renderProjKpis) -->
    <div id="pfin-wf-cards" style="display:none;flex-shrink:0;"></div>
    <!-- Quick actions -->
    <div class="pfin-actions" style="flex-shrink:0;">
      <button class="pfin-btn pfin-btn-income" onclick="openAddPayment()"><i class="ti ti-plus"></i> إضافة دفعة</button>
      <button class="pfin-btn pfin-btn-expense" onclick="openAddExpense()"><i class="ti ti-minus"></i> إضافة مصروف</button>
      <button class="pfin-btn pfin-btn-print" onclick="printProjStatement()"><i class="ti ti-printer"></i> طباعة كشف الحساب</button>
      <button class="pfin-btn pfin-btn-export" onclick="exportProjCsv()"><i class="ti ti-file-spreadsheet"></i> تصدير CSV</button>
      <div style="margin-right:auto;display:flex;align-items:center;gap:8px;">
        <span id="pfin-currency-label" style="font-size:12px;color:rgba(255,255,255,0.7);">العملة: <strong id="pfin-currency-display" style="color:#fff;">—</strong></span>
        <input type="hidden" id="pfin-currency" value='USD'>
      </div>
    </div>
    <!-- Tabs -->
    <div class="pfin-tabs" style="flex-shrink:0;">
      <div class="pfin-tab on" id="pfin-tab-all" onclick="switchPfinTab('all')">كل الحركات</div>
      <div class="pfin-tab" id="pfin-tab-income" onclick="switchPfinTab('income')">💰 دفعات العميل</div>
      <div class="pfin-tab" id="pfin-tab-expense" onclick="switchPfinTab('expense')">📤 المصروفات</div>
    </div>
    <!-- Ledger -->
    <div style="flex:1;overflow-y:auto;">
      <div class="pfin-ledger" id="pfin-ledger"></div>
    </div>
    <div class="mft" style="flex-shrink:0;">
      <button class="btn-cancel" onclick="closeProjFin()">إغلاق</button>
    </div>
  </div>
</div>

<!-- ══ ADD PAYMENT MODAL ══════════════════════════════════════════════ -->
<div class="overlay" id="add-pay-overlay" onclick="if(event.target===this)closeAddPayment()">
  <div class="modal fin-quick-modal" onclick="event.stopPropagation()" style="width:460px;">
    <div class="mhd">
      <div>
        <div class="mhd-t" style="color:var(--green);">💰 تسجيل دفعة من العميل</div>
        <div class="mhd-sub" id="add-pay-sub"></div>
      </div>
      <button class="icon-btn" onclick="closeAddPayment()" style="display:flex;align-items:center;gap:4px;padding:5px 10px;border-radius:6px;"><i class="ti ti-x"></i> إغلاق</button>
    </div>
    <div class="mbody">
      <div class="fg fin-amount-big">
        <label>المبلغ المستلم <span class="req">*</span></label>
        <div style="display:flex;gap:8px;">
          <input class="fi" type="number" id="pay-amount" min="0" placeholder="0" oninput="updatePayRemaining()">
          <select class="fi" id="pay-currency" style="display:none;">
            <option value='USD'>$</option>
            <option value="USD">$</option>
            <option value="SYP">ل.س</option>
          </select>
          <span id="pay-currency-label" style="font-size:15px;font-weight:700;color:var(--accent);min-width:40px;">$</span>
        </div>
        <div id="pay-remaining-hint" style="margin-top:6px;font-size:12px;color:var(--text3);"></div>
      </div>
      <div class="frow">
        <div class="fg">
          <label>تاريخ الاستلام <span class="req">*</span></label>
          <input class="fi" type="date" id="pay-date">
        </div>
        <div class="fg">
          <label>وصف / رقم الدفعة</label>
          <input class="fi" id="pay-label" placeholder="مثل: دفعة أولى، دفعة مقدمة...">
        </div>
      </div>
      <div class="fg">
        <label>ملاحظات</label>
        <textarea class="fi" id="pay-notes" placeholder="أي ملاحظات..." style="min-height:60px;"></textarea>
      </div>
      <div class="fg">
        <label>صورة إيصال الاستلام</label>
        <div class="receipt-drop" onclick="document.getElementById('pay-receipt-inp').click()">
          <i class="ti ti-receipt"></i>
          <span>اضغط لرفع صورة الإيصال أو الشيك</span>
        </div>
        <input type="file" id="pay-receipt-inp" accept=".jpg,.jpeg,.png,.webp,.pdf" style="display:none;" onchange="onPayReceiptSelected()">
        <div class="receipt-preview-wrap" id="pay-receipt-preview" style="display:none;"></div>
      </div>
    </div>
    <div class="mft">
      <button class="btn-cancel" onclick="closeAddPayment()">إلغاء</button>
      <button class="btn-save" style="background:var(--green);" onclick="savePayment()">
        <i class="ti ti-check" style="vertical-align:-2px;margin-left:4px;"></i> تأكيد الاستلام
      </button>
    </div>
  </div>
</div>

<!-- ══ ADD EXPENSE MODAL ══════════════════════════════════════════════ -->
<div class="overlay" id="add-exp-overlay" onclick="if(event.target===this)closeAddExpense()">
  <div class="modal fin-quick-modal modal-wide" onclick="event.stopPropagation()">
    <div class="mhd">
      <div>
        <div class="mhd-t" style="color:var(--red);">📤 تسجيل مصروف</div>
        <div class="mhd-sub" id="add-exp-sub"></div>
      </div>
      <button class="icon-btn" onclick="closeAddExpense()" style="display:flex;align-items:center;gap:4px;padding:5px 10px;border-radius:6px;"><i class="ti ti-x"></i> إغلاق</button>
    </div>
    <div class="mbody">
      <div class="fg">
        <label>تصنيف المصروف <span class="req">*</span></label>
        <div class="expense-cat-grid" id="exp-cat-grid">
          <button class="exp-cat-btn" data-cat="materials" onclick="selExpCat(this)"><span class="cat-icon">🧱</span>مواد</button>
          <button class="exp-cat-btn" data-cat="labor"     onclick="selExpCat(this)"><span class="cat-icon">👷</span>أجور عمال</button>
          <button class="exp-cat-btn" data-cat="municipal" onclick="selExpCat(this)"><span class="cat-icon">🏛️</span>رسوم بلدية</button>
          <button class="exp-cat-btn" data-cat="license"   onclick="selExpCat(this)"><span class="cat-icon">📜</span>رسوم تراخيص</button>
          <button class="exp-cat-btn" data-cat="transport" onclick="selExpCat(this)"><span class="cat-icon">🚗</span>نقل ومواصلات</button>
          <button class="exp-cat-btn" data-cat="sitevisit" onclick="selExpCat(this)"><span class="cat-icon">📍</span>زيارات ميدانية</button>
          <button class="exp-cat-btn" data-cat="admin"     onclick="selExpCat(this)"><span class="cat-icon">📊</span>إدارية</button>
          <button class="exp-cat-btn" data-cat="other"     onclick="selExpCat(this)"><span class="cat-icon">📦</span>أخرى</button>
        </div>
        <input type="hidden" id="exp-category" value="">
      </div>
      <div class="frow">
        <div class="fg fin-amount-big">
          <label>المبلغ <span class="req">*</span></label>
          <div style="display:flex;gap:8px;">
            <input class="fi" type="number" id="exp-amount" min="0" placeholder="0">
            <select class="fi" id="exp-currency" style="width:100px;">
              <option value='USD'>$</option>
              <option value="USD">$</option>
              <option value="SYP">ل.س</option>
            </select>
          </div>
        </div>
        <div class="fg">
          <label>تاريخ المصروف <span class="req">*</span></label>
          <input class="fi" type="date" id="exp-date">
        </div>
      </div>
      <div class="fg">
        <label>وصف المصروف <span class="req">*</span></label>
        <input class="fi" id="exp-label" placeholder="مثل: شراء حديد، أجرة نقل، رسوم ترخيص...">
      </div>
      <div class="fg">
        <label>ملاحظات</label>
        <textarea class="fi" id="exp-notes" placeholder="(اختياري)" style="min-height:55px;"></textarea>
      </div>
      <div class="fg">
        <label>صورة الفاتورة أو الإيصال</label>
        <div class="receipt-drop" onclick="document.getElementById('exp-receipt-inp').click()">
          <i class="ti ti-file-invoice"></i>
          <span>اضغط لرفع صورة الفاتورة أو الإيصال</span>
        </div>
        <input type="file" id="exp-receipt-inp" accept=".jpg,.jpeg,.png,.webp,.pdf" style="display:none;" onchange="onExpReceiptSelected()">
        <div class="receipt-preview-wrap" id="exp-receipt-preview" style="display:none;"></div>
      </div>
    </div>
    <div class="mft">
      <button class="btn-cancel" onclick="closeAddExpense()">إلغاء</button>
      <button class="btn-save" style="background:var(--red);" onclick="saveExpense()">
        <i class="ti ti-check" style="vertical-align:-2px;margin-left:4px;"></i> حفظ المصروف
      </button>
    </div>
  </div>
</div>

<!-- ══ CLIENT FINANCE MODAL ══════════════════════════════════════════ -->
<div class="overlay" id="cfin-overlay" onclick="if(event.target===this)closeCFin()">
  <div class="modal modal-wide" onclick="event.stopPropagation()">
    <div class="mhd">
      <div>
        <div class="mhd-t" id="cfin-title">ملخص العميل المالي</div>
        <div class="mhd-sub" id="cfin-sub"></div>
      </div>
      <button class="icon-btn" onclick="closeCFin()" style="display:flex;align-items:center;gap:4px;padding:5px 10px;border-radius:6px;"><i class="ti ti-x"></i> إغلاق</button>
    </div>
    <div class="mbody" id="cfin-body" style="gap:0;padding:0;"></div>
    <div class="mft">
      <button class="tbtn" onclick="printClientStatement()"><i class="ti ti-printer"></i> طباعة كشف العميل</button>
      <button class="btn-cancel" onclick="closeCFin()">إغلاق</button>
    </div>
  </div>
</div>

<!-- ══ RECEIPT LIGHTBOX ══════════════════════════════════════════════ -->
<div class="overlay" id="lightbox-overlay" onclick="closeLightbox()" style="background:rgba(0,0,0,.85);align-items:center;justify-content:center;">
  <img id="lightbox-img" style="max-width:90vw;max-height:90vh;border-radius:8px;box-shadow:0 8px 40px rgba(0,0,0,.6);">
</div>

<!-- ══ CLIENT MODAL (Add / Edit) ═══════════════════════════════════ -->
<div class="overlay" id="client-overlay" onclick="if(event.target===this)closeClientModal()">
  <div class="modal" onclick="event.stopPropagation()">
    <div class="mhd">
      <div>
        <div class="mhd-t" id="client-modal-title">إضافة عميل جديد</div>
        <div class="mhd-sub" id="client-modal-code"></div>
      </div>
      <button class="icon-btn" onclick="closeClientModal()" style="display:flex;align-items:center;gap:4px;padding:5px 10px;border-radius:6px;"><i class="ti ti-x"></i> إغلاق</button>
    </div>
    <div class="mbody">
      <div class="frow">
        <div class="fg">
          <label>اسم العميل <span class="req">*</span></label>
          <input class="fi" id="client-name" placeholder="الاسم الكامل للعميل...">
        </div>
        <div class="fg">
          <label>رقم العميل</label>
          <input class="fi" id="client-code-display" readonly placeholder="تلقائي">
        </div>
      </div>
      <div class="frow">
        <div class="fg">
          <label>رقم الهاتف <span class="req">*</span></label>
          <input class="fi" id="client-phone" placeholder="+963...">
        </div>
        <div class="fg">
          <label>واتساب</label>
          <input class="fi" id="client-whatsapp" placeholder="+963... (اختياري)">
        </div>
      </div>
      <div class="fg">
        <label>البريد الإلكتروني</label>
        <input class="fi" type="email" id="client-email" placeholder="(اختياري)">
      </div>
      <div class="fg">
        <label>العنوان / المنطقة</label>
        <input class="fi" id="client-address" placeholder="(اختياري)">
      </div>
      <div class="fg">
        <label>ملاحظات</label>
        <textarea class="fi" id="client-notes" placeholder="أي ملاحظات إضافية..." style="min-height:70px;"></textarea>
      </div>
    </div>
    <div class="mft">
      <button class="btn-cancel" onclick="closeClientModal()">إلغاء</button>
      <button class="btn-save" onclick="saveClient()">
        <i class="ti ti-device-floppy" style="vertical-align:-2px;margin-left:4px;"></i> حفظ
      </button>
    </div>
  </div>
</div>

<!-- ══ ADD ENGINEER MODAL ════════════════════════════════════════════ -->
<div class="overlay" id="eng-modal" onclick="if(event.target===this)closeEngModal()">
  <div class="modal" onclick="event.stopPropagation()">
    <div class="mhd">
      <div class="mhd-t">إضافة مهندس</div>
      <button class="icon-btn" onclick="closeEngModal()" style="display:flex;align-items:center;gap:4px;padding:5px 10px;border-radius:6px;"><i class="ti ti-x"></i> إغلاق</button>
    </div>
    <div class="mbody">
      <div class="fg"><label>الاسم الكامل <span class="req">*</span></label><input class="fi" id="eng-name" placeholder="اسم المهندس..."></div>
      <div class="frow">
        <div class="fg"><label>رقم الهاتف</label><input class="fi" id="eng-phone" placeholder="+9665..."></div>
        <div class="fg"><label>واتساب</label><input class="fi" id="eng-wa" placeholder="+9665..."></div>
      </div>
      <div class="fg"><label>البريد الإلكتروني</label><input class="fi" id="eng-email" type="email" placeholder="(اختياري)"></div>
    </div>
    <div class="mft">
      <button class="btn-cancel" onclick="closeEngModal()">إلغاء</button>
      <button class="btn-save" onclick="saveEngineer()">إضافة</button>
    </div>
  </div>
</div>

<div class="toast" id="toast"></div>

<!-- ═══ Followup / Tracking Modal ═══ -->
<div class="overlay" id="fu-overlay" onclick="if(event.target===this)closeFollowup()">
  <div class="modal modal-wide" onclick="event.stopPropagation()" style="max-height:92vh;display:flex;flex-direction:column;width:min(1100px,95vw);">
    <div class="modal-header" style="display:flex;align-items:center;justify-content:space-between;padding:14px 18px;border-bottom:1px solid #eee;">
      <div>
        <div style="font-size:18px;font-weight:700;" id="fu-title">متابعة المشروع</div>
        <div style="font-size:12px;color:#666;" id="fu-subtitle"></div>
      </div>
      <button class="icon-btn" onclick="closeFollowup()" style="display:flex;align-items:center;gap:4px;padding:5px 10px;border-radius:6px;"><i class="ti ti-x"></i> إغلاق</button>
    </div>
    <div id="fu-body" style="overflow:auto;padding:16px 18px;flex:1;"></div>
  </div>
</div>

<style>
.fu-tabs{display:flex;gap:6px;border-bottom:1px solid #e5e7eb;margin-bottom:14px;flex-wrap:wrap;}
.fu-tab{padding:8px 14px;cursor:pointer;border-radius:8px 8px 0 0;font-size:13px;color:#555;border:1px solid transparent;border-bottom:none;}
.fu-tab.active{background:#f3f6fb;color:#1e40af;border-color:#dbe3ee;font-weight:600;}
.fu-phase{border:1px solid #e5e7eb;border-radius:10px;margin-bottom:10px;background:#fff;overflow:hidden;}
.fu-phase-head{display:flex;align-items:center;justify-content:space-between;padding:10px 14px;cursor:pointer;background:#fafbfc;}
.fu-phase-head:hover{background:#f3f6fb;}
.fu-phase-title{font-weight:600;font-size:14px;display:flex;align-items:center;gap:10px;}
.fu-phase-body{padding:14px;border-top:1px solid #eee;display:none;}
.fu-phase.open .fu-phase-body{display:block;}
.fu-mini{display:grid;grid-template-columns:repeat(auto-fit,minmax(180px,1fr));gap:10px;margin-bottom:10px;}
.fu-mini label{font-size:11px;color:#666;display:block;margin-bottom:3px;}
.fu-mini input,.fu-mini select,.fu-mini textarea{width:100%;padding:6px 8px;border:1px solid #d1d5db;border-radius:6px;font-size:13px;font-family:inherit;}
.fu-section-title{font-size:13px;font-weight:700;margin:14px 0 8px;color:#1e40af;display:flex;align-items:center;gap:6px;}
.fu-btn{padding:6px 12px;border:1px solid #d1d5db;background:#fff;border-radius:6px;cursor:pointer;font-size:12px;display:inline-flex;align-items:center;gap:5px;}
.fu-btn:hover{background:#f3f6fb;}
.fu-btn-primary{background:#2563eb;color:#fff;border-color:#2563eb;}
.fu-btn-primary:hover{background:#1d4ed8;}
.fu-btn-danger{color:#dc2626;border-color:#fecaca;}
.fu-row{display:flex;gap:8px;align-items:center;padding:6px 10px;background:#fafbfc;border:1px solid #eee;border-radius:6px;margin-bottom:5px;font-size:13px;}
.fu-row input[type=text],.fu-row input[type=tel],.fu-row input[type=number]{flex:1;padding:4px 6px;border:1px solid #d1d5db;border-radius:4px;font-size:12px;}
.fu-file-item{display:flex;align-items:center;justify-content:space-between;padding:8px 10px;background:#fff;border:1px solid #e5e7eb;border-radius:6px;margin-bottom:5px;font-size:12px;}
.fu-file-meta{color:#666;font-size:11px;}
.fu-vbadge{padding:2px 8px;border-radius:10px;font-size:10px;font-weight:600;}
.fu-v-pending{background:#fef3c7;color:#92400e;}
.fu-v-approved{background:#d1fae5;color:#065f46;}
.fu-v-revise{background:#fee2e2;color:#991b1b;}
.fu-issue{border:1px solid #fecaca;background:#fef2f2;border-radius:6px;padding:8px;margin-bottom:6px;font-size:12px;}
.fu-log{border:1px solid #e5e7eb;border-radius:8px;padding:10px;margin-bottom:8px;background:#fff;}
.fu-prog{height:6px;background:#e5e7eb;border-radius:3px;overflow:hidden;flex:1;max-width:120px;}
.fu-prog-fill{height:100%;background:linear-gradient(90deg,#3b82f6,#06b6d4);}
</style>

<script>
// ══════════════════════════════════════════════════════════════════
// STATE
// ══════════════════════════════════════════════════════════════════
let CU = null; // current user
let ET_VIEW = 'normal'; // 'normal' | 'byengineer'
let SETTINGS = {
  company: { name:'مكتب ProjexID الهندسي', phone:'', email:'', address:'', city:'', country:'سوريا', website:'', logo:null },
  finance: { defaultCurrency:'USD', paymentMethods:['نقداً','تحويل بنكي','شيك','تحويل إلكتروني'], vatEnabled:false, vatRate:0 },
  reports: { prefix:'REP', showLogo:true, showEngineer:true, showPhotos:true, showSignature:false, showNotes:true, showClient:true },
  dashboard: { showProjects:true, showReports:true, showFinance:true },
  workshopTypes: ['ورشة لياسة','ورشة كهرباء','ورشة سباكة','ورشة ألمنيوم','ورشة نجارة','ورشة سيراميك','ورشة دهانات','ورشة حفريات'],
  workerTypes:   ['نجار','حداد','كهربائي','سباك','دهان','عامل عادي','فورمان'],
  sessionTimeout: 0
};
let ACTIVITY_LOG = []; // [{id, user, action, time}]
let SET_TAB = 'company'; // active settings tab
let DUSERS  = null;      // dynamic users (loaded from localStorage)

// All available permissions
const ALL_PERMS = [
  { key:'view_projects',   ar:'مشاهدة المشاريع',       group:'عرض' },
  { key:'view_clients',    ar:'مشاهدة العملاء',         group:'عرض' },
  { key:'view_finance',    ar:'الشؤون المالية',          group:'عرض' },
  { key:'view_reports',    ar:'مشاهدة التقارير',         group:'عرض' },
  { key:'view_daily',      ar:'السجل اليومي',            group:'عرض' },
  { key:'view_workers',    ar:'مشاهدة العمال والورشات',  group:'عرض' },
  { key:'view_settings',   ar:'الإعدادات',              group:'عرض' },
  { key:'add_projects',    ar:'إضافة مشاريع',            group:'تعديل' },
  { key:'edit_projects',   ar:'تعديل المشاريع',          group:'تعديل' },
  { key:'delete_projects', ar:'حذف المشاريع',            group:'تعديل' },
  { key:'manage_clients',  ar:'إدارة العملاء (إضافة/حذف)', group:'تعديل' },
  { key:'manage_payments', ar:'إدارة الدفعات المالية',  group:'تعديل' },
  { key:'approve_reports', ar:'اعتماد وإرسال التقارير', group:'تعديل' },
  { key:'manage_workforce',ar:'إدارة العمال والورشات',   group:'تعديل' },
];

// Default permission sets per role
const ROLE_DEFAULT_PERMS = {
  manager:    { view_projects:1,view_clients:1,view_finance:1,view_reports:1,view_daily:1,view_workers:1,view_settings:1,add_projects:1,edit_projects:1,delete_projects:1,manage_clients:1,manage_payments:1,approve_reports:1,manage_workforce:1 },
  engineer:   { view_projects:1,view_reports:1,view_daily:1,view_workers:1,approve_reports:1,manage_workforce:1 },
  accountant: { view_projects:1,view_clients:1,view_finance:1,view_reports:1,manage_payments:1 },
  viewer:     { view_projects:1,view_clients:1,view_reports:1 },
};

function hasPermission(perm) {
  if(!CU) return false;
  if(CU.role==='manager') return true; // manager always has all
  return !!(CU.permissions?.[perm]);
}
let DB = null; // IndexedDB
let STATE = {
  clients: [],
  projects: [],
  engineers: [],
  reports: [],
  finance: {}
};

// Work-order editing
let WO_EDIT_ID = null;
let WO_FILES = [];
let WO_PAYMENTS = [];
let FIN_EDIT_ID = null;
let FIN_PAYMENTS = [];
let ENG_UPD_ID = null;

// Type config
const TYPES = {
  design: { ar: 'تصميم', icon: '🎨', prefix: 'PRD', badge: 'badge-design' },
  permit: { ar: 'رخصة بناء', icon: '📋', prefix: 'PRP', badge: 'badge-permit' },
  super:  { ar: 'إشراف', icon: '👁️', prefix: 'PRS', badge: 'badge-super' },
  exec:   { ar: 'تنفيذ', icon: '🔨', prefix: 'PRE', badge: 'badge-exec' },
  admin:  { ar: 'إدارية', icon: '📊', prefix: 'PRA', badge: 'badge-admin' }
};

const STATUS = {
  waiting:    { ar: 'قائمة الانتظار', badge: 'badge-waiting' },
  inprog:     { ar: 'قيد التنفيذ', badge: 'badge-inprog' },
  review:     { ar: 'قيد المراجعة', badge: 'badge-review' },
  done:       { ar: 'مكتمل', badge: 'badge-done' },
  hold:       { ar: 'متوقف', badge: 'badge-hold' },
  waitclient: { ar: 'انتظار العميل', badge: 'badge-waitclient' }
};

const PRI = {
  urgent: { ar: 'عاجل', badge: 'badge-urgent' },
  medium: { ar: 'متوسط', badge: 'badge-medium' },
  low:    { ar: 'منخفض', badge: 'badge-low' }
};

// Two currencies only: USD and SYP
const CURRENCY_SYMBOL = { USD: '$', SYP: 'ل.س' };
const DEFAULT_CURRENCY = 'USD';

// Approximate cross-currency rate for global overview display only
const CROSS_RATE_SYP_TO_USD = 1 / 14500; // 1 USD ≈ 14,500 SYP (used only for global sums)

// ── Exec type detection ──────────────────────────────────────────
function isExecType(p) {
  return p && (p.taskTypeKey === 'exec' || p.taskTypeKey === 'super');
}

// ── Workforce calculation helpers ─────────────────────────────────
function spTotal(s) {
  // Workshop total: prefer qty × unitPrice, fallback to contractValue
  if ((s.qty||0) > 0 && (s.unitPrice||0) > 0) return (s.qty||0) * (s.unitPrice||0);
  return s.contractValue || 0;
}
function spPaid(s) {
  return (s.payments||[]).reduce((a, pm) => a + (pm.amount||0), 0);
}
function wkTotal(w) {
  return (w.dailyWage||0) * (w.days||0);
}
function wkPaid(w) {
  return (w.payments||[]).reduce((a, pm) => a + (pm.amount||0), 0);
}
function calcWorkforceTotals(p) {
  const wk = p.workforce || {};
  let wsContract=0, wsPaid=0, wkCost=0, wkPaidAmt=0;
  (wk.workshops||[]).forEach(s => { wsContract += spTotal(s); wsPaid += spPaid(s); });
  (wk.workers||[]).forEach(w  => { wkCost    += wkTotal(w);  wkPaidAmt += wkPaid(w); });
  return {
    wsContract, wsPaid,   wsRem: wsContract - wsPaid,
    wkCost,     wkPaidAmt, wkRem: wkCost - wkPaidAmt,
    total: wsContract + wkCost,
    totalPaid: wsPaid + wkPaidAmt,
    totalRem: (wsContract - wsPaid) + (wkCost - wkPaidAmt),
  };
}
// Trigger finance refresh if finance modal or main finance view is open
function wfSyncFinance() {
  if (document.getElementById('pfin-overlay')?.classList.contains('open')
      && PFIN_PROJECT_ID === FU_CUR) {
    renderProjKpis();
  }
  // Also refresh finance section if it's visible
  const finView = document.getElementById('view-finance');
  if (finView?.classList.contains('on')) {
    renderFinance();
  }
}

// fmt shim removed

function formatAmount(value, currency) {
  return fmt(value, currency);
}

function toUSD(amount, currency) {
  // Approximate conversion to USD for global summaries only
  if (currency === 'USD' || !currency) return amount || 0;
  if (currency === 'SYP') return Math.round((amount || 0) * CROSS_RATE_SYP_TO_USD);
  return amount || 0;
}

const REP_TYPES = {
  daily:     { ar: 'يومي' },
  weekly:    { ar: 'أسبوعي' },
  milestone: { ar: 'مرحلي' },
  final:     { ar: 'نهائي' }
};

// ══════════════════════════════════════════════════════════════════
// STORAGE — Multi-layer (localStorage + memory fallback)
// ══════════════════════════════════════════════════════════════════
let DB = null;
const MEM_STORE = {}; // in-memory fallback
let USE_LS = true;

// Test if localStorage actually works
(function() {
  try {
    localStorage.setItem('__pxid_test__', '1');
    const v = localStorage.getItem('__pxid_test__');
    localStorage.removeItem('__pxid_test__');
    USE_LS = (v === '1');
  } catch(e) {
    USE_LS = false;
  }
})();

function initDB() { return Promise.resolve(); }

function lsKey(store) { return 'pxid_store_' + store; }

function lsGetAll(store) {
  // Try localStorage first
  if (USE_LS) {
    try {
      const raw = localStorage.getItem(lsKey(store));
      if (raw) {
        const parsed = JSON.parse(raw);
        MEM_STORE[store] = parsed; // sync to memory
        return parsed;
      }
    } catch(e) { USE_LS = false; }
  }
  // Fallback to memory
  return MEM_STORE[store] ? [...MEM_STORE[store]] : [];
}

function lsSave(store, items) {
  MEM_STORE[store] = [...items]; // always save to memory
  if (USE_LS) {
    try {
      localStorage.setItem(lsKey(store), JSON.stringify(items));
    } catch(e) {
      USE_LS = false;
      // Try saving smaller chunks if quota exceeded
      try {
        // Remove old data and retry
        for (const k of Object.keys(localStorage)) {
          if (k.startsWith('pxid_store_') && k !== lsKey(store)) {
            // Keep other stores
          }
        }
        localStorage.setItem(lsKey(store), JSON.stringify(items));
        USE_LS = true;
      } catch(e2) {
        console.warn('localStorage unavailable, using memory only');
      }
    }
  }
}

async function dbGetAll(store) {
  return Promise.resolve(lsGetAll(store));
}

async function dbPut(store, obj) {
  const items = lsGetAll(store);
  const idx = items.findIndex(x => String(x.id) === String(obj.id));
  if (idx >= 0) items[idx] = obj;
  else items.push(obj);
  lsSave(store, items);
  return Promise.resolve();
}

async function dbDelete(store, id) {
  const items = lsGetAll(store).filter(x => String(x.id) !== String(id));
  lsSave(store, items);
  return Promise.resolve();
}

async function loadAllData() {
  STATE.clients   = await dbGetAll('clients');
  STATE.engineers = await dbGetAll('engineers');
  STATE.projects  = await dbGetAll('projects');
  STATE.reports   = await dbGetAll('reports');
  if (STATE.engineers.length === 0) {
    const defaults = [
      {id:1001,name:'أحمد الرشيدي',phone:'+966501234567',whatsapp:'+966501234567',email:'ahmed@example.com',createdAt:Date.now()},
      {id:1002,name:'سارة المحمود',phone:'+966502345678',whatsapp:'+966502345678',email:'sara@example.com',createdAt:Date.now()},
      {id:1003,name:'نور الحسيني',phone:'+966503456789',whatsapp:'+966503456789',email:'nour@example.com',createdAt:Date.now()}
    ];
    for (const e of defaults) await dbPut('engineers', e);
    STATE.engineers = defaults;
  }
}

// ══════════════════════════════════════════════════════════════════
// LOGIN / LOGOUT
// ══════════════════════════════════════════════════════════════════
document.getElementById('l-pass').addEventListener('keydown', e => { if(e.key==='Enter') doLogin(); });
document.getElementById('l-user').addEventListener('keydown', e => { if(e.key==='Enter') doLogin(); });

// ── User accounts ─────────────────────────────────────────────────
const USERS = [
  { username:'osman', password:'osman', role:'manager',  name:'Osman',      avatar:'أ' },
  { username:'eng',   password:'eng',   role:'engineer', name:'المهندس',     avatar:'م' },
];

// ── Views/actions forbidden for each role ──────────────────────
const ROLE_BLOCKED = {
  engineer: new Set(['finance','clients','settings']),
};

// Apply UI based on current role
function applyRoleUI() {
  if(!CU) return;
  const isMgr = CU.role === 'manager';

  // Nav visibility driven by per-user permissions
  const canClients  = hasPermission('view_clients');
  const canFinance  = hasPermission('view_finance');
  const canSettings = hasPermission('view_settings');

  const vis = {
    'nav-clients':    canClients,
    'nav-settings':   canSettings,
    'nav-finance':    canFinance,
    'sb-admin-sec':   canClients,
    'sb-system-sec':  canSettings,
    'sb-finance-sec': canFinance,
  };
  Object.entries(vis).forEach(([id, show]) => {
    const el = document.getElementById(id);
    if(el) el.style.display = show ? '' : 'none';
  });

  // User badge
  const uav  = document.getElementById('u-av');
  const uname= document.getElementById('u-name');
  const urole= document.getElementById('u-role');
  if(uav)   uav.textContent   = CU.avatar;
  if(uname) uname.textContent = CU.name;
  if(urole) urole.textContent = isMgr ? 'مدير المشاريع' : 'مهندس';

  // Topbar buttons
  const btnTask = document.getElementById('btn-add-task');
  const btnRep  = document.getElementById('btn-add-report');
  if(btnTask) btnTask.style.display = isMgr ? 'flex' : 'none';
  if(btnRep)  btnRep.style.display  = 'none';
}

async function doLogin() {
  const u   = document.getElementById('l-user').value.trim().toLowerCase();
  const p   = document.getElementById('l-pass').value;
  const err = document.getElementById('l-err');
  err.textContent = '';

  const user = USERS.find(x => x.username === u && x.password === p);
  if (!user) {
    err.textContent = '⚠ اسم المستخدم أو كلمة المرور غير صحيحة';
    document.getElementById('l-pass').value = '';
    return;
  }

  // Build permissions: use stored user.permissions or role defaults
  const perms = user.permissions || {...(ROLE_DEFAULT_PERMS[user.role]||ROLE_DEFAULT_PERMS.viewer)};
  CU = { name: user.name, username: user.username, role: user.role, avatar: user.avatar, permissions: perms };

  // Persist session
  try { localStorage.setItem('pxid_session', JSON.stringify(CU)); } catch(e){}

  await initDB();
  await loadAllData();

  document.getElementById('login-wrap').style.display = 'none';
  document.getElementById('app').style.display = 'flex';
  applyRoleUI();
  renderAll();
  logActivity('تسجيل دخول');
}

// ── Restore session on page load ─────────────────────────────────
function tryRestoreSession() {
  try {
    const saved = localStorage.getItem('pxid_session');
    if (!saved) return false;
    const parsed = JSON.parse(saved);
    // Validate the saved user still exists
    const valid = USERS.find(x => x.username === parsed.username);
    if (!valid) { localStorage.removeItem('pxid_session'); return false; }
    // Restore permissions from saved session or rebuild from DUSERS
    const savedUser = (DUSERS||[]).find(u=>u.username===parsed.username);
    if(savedUser?.permissions) parsed.permissions = savedUser.permissions;
    else if(!parsed.permissions) parsed.permissions = {...(ROLE_DEFAULT_PERMS[parsed.role]||{})};
    CU = parsed;
    return true;
  } catch(e) { return false; }
}

function doLogout() {
  CU = null;
  try { localStorage.removeItem('pxid_session'); } catch(e){}
  document.getElementById('login-wrap').style.display='flex';
  document.getElementById('app').style.display='none';
  document.getElementById('l-user').value='';
  document.getElementById('l-pass').value='';
  document.getElementById('l-err').textContent='';
}

// ══════════════════════════════════════════════════════════════════
// NAVIGATION
// ══════════════════════════════════════════════════════════════════
const PAGE_TITLES = { dashboard:'الصفحة الرئيسية', clients:'العملاء', projects:'المشاريع', 'eng-tasks':'مهام المهندسين', 'proj-followup':'متابعة المشاريع', finance:'الشؤون المالية', reports:'التقارير', settings:'الإعدادات' };

function sw(name, el) {
  // Permission-based access control
  const permMap = { finance:'view_finance', clients:'view_clients', settings:'view_settings' };
  if (CU && permMap[name] && !hasPermission(permMap[name])) {
    toast('⛔ ليس لديك صلاحية للوصول إلى هذا القسم');
    return;
  }
  document.querySelectorAll('.view').forEach(v => v.classList.remove('on'));
  document.querySelectorAll('.ni[data-view]').forEach(n => n.classList.remove('on'));
  document.getElementById('view-'+name)?.classList.add('on');
  el?.classList.add('on');
  document.getElementById('pg-title').textContent = PAGE_TITLES[name]||'';
  // topbar buttons
  document.getElementById('btn-add-task').style.display = (CU?.role==='manager' && name!=='reports' && name!=='settings' && name!=='clients')?'flex':'none';
  const btnAddClient = document.getElementById('btn-add-client');
  if(btnAddClient) btnAddClient.style.display = (CU?.role==='manager' && name==='clients')?'flex':'none';
  document.getElementById('btn-add-report').style.display = (CU?.role==='engineer' && name==='reports')?'flex':'none';
  if (name==='dashboard')  renderDashboard();
  if (name==='clients')    renderClients();
  if (name==='projects')   renderProjects();
  if (name==='eng-tasks') {
    renderEngTasks();
    // Restore correct sub-view
    if(ET_VIEW === 'byengineer') {
      document.getElementById('eng-tasks-list')?.style.setProperty('display','none');
      const byEngEl = document.getElementById('eng-tasks-byeng');
      if(byEngEl) { byEngEl.style.display=''; }
      renderEngTasksByEngineer();
    } else {
      document.getElementById('eng-tasks-list')?.style.setProperty('display','');
      document.getElementById('eng-tasks-byeng')?.style.setProperty('display','none');
    }
    // Sync toggle buttons
    ['normal','byengineer'].forEach(v=>{
      document.getElementById('et-vbtn-'+v)?.classList.toggle('on', v===ET_VIEW);
    });
  }
  if (name==='finance')    renderFinance();
  if (name==='reports') {
    renderReports();
    // Sync group toggle buttons
    ['none','project','client','engineer'].forEach(g=>{
      document.getElementById('rg-'+g)?.classList.toggle('on', g===REP_GROUP);
    });
    const repBackBtn = document.getElementById('rep-back-btn');
    if(repBackBtn) repBackBtn.style.display = REP_GROUP!=='none' ? '' : 'none';
    const filterBar = document.getElementById('rep-filter-bar');
    if(filterBar) filterBar.style.display = REP_GROUP==='none' ? '' : 'none';
  }
  if (name==='settings')     renderSettings();
  if (name==='proj-followup') renderProjFollowup();
}

function renderAll() {
  updateBadges();
  renderDashboard();
  sw('dashboard', document.querySelector('.ni[data-view=dashboard]'));
}

function updateBadges() {
  const active = STATE.projects.filter(p => p.status!=='done').length;
  document.getElementById('badge-tasks').textContent = active||'';
  if(!active) document.getElementById('badge-tasks').style.display='none';
  else document.getElementById('badge-tasks').style.display='';
}

// ══════════════════════════════════════════════════════════════════
// DASHBOARD
// ══════════════════════════════════════════════════════════════════
function renderDashboard() {
  const P = STATE.projects;
  const total = P.length;
  const active = P.filter(p=>p.status==='inprog').length;
  const done = P.filter(p=>p.status==='done').length;
  const overdue = P.filter(p=>p.deliveryDate && p.status!=='done' && new Date(p.deliveryDate)<new Date()).length;

  document.getElementById('dash-stats').innerHTML = `
    <div class="stat-card sc-blue">
      <div class="stat-icon" style="background:var(--blue-light);"><i class="ti ti-users" style="color:var(--blue);"></i></div>
      <div class="stat-val">${STATE.clients.length}</div>
      <div class="stat-lbl">إجمالي العملاء</div>
      <div class="stat-sub" style="color:var(--blue);">${P.length} مشروع مرتبط</div>
    </div>
    <div class="stat-card sc-green">
      <div class="stat-icon" style="background:var(--green-light);"><i class="ti ti-folder-open" style="color:var(--green);"></i></div>
      <div class="stat-val">${total}</div>
      <div class="stat-lbl">إجمالي المشاريع</div>
      <div class="stat-sub" style="color:var(--green);">${active} نشط</div>
    </div>
    <div class="stat-card sc-amber">
      <div class="stat-icon" style="background:var(--amber-light);"><i class="ti ti-check" style="color:var(--amber);"></i></div>
      <div class="stat-val">${done}</div>
      <div class="stat-lbl">مشاريع مكتملة</div>
      <div class="stat-sub" style="color:var(--amber);">${total?Math.round(done/total*100):0}% من الإجمالي</div>
    </div>
    <div class="stat-card sc-red">
      <div class="stat-icon" style="background:var(--red-light);"><i class="ti ti-alert-triangle" style="color:var(--red);"></i></div>
      <div class="stat-val">${overdue}</div>
      <div class="stat-lbl">متأخرة التسليم</div>
      <div class="stat-sub" style="color:var(--red);">${overdue>0?'تحتاج اهتماماً':'لا تأخيرات!'}</div>
    </div>`;

  // Type chart
  const chartHtml = `<div class="dash-type-grid">` + Object.entries(TYPES)
    .map(([k, info]) => {
      const projects = P.filter(p => p.taskTypeKey === k);
      const totalByType = projects.length;
      const completedByType = projects.filter(p => p.status === 'done').length;
      const finishedByType = projects.filter(p => (p.progress || 0) >= 100).length;
      const itemsHtml = projects.length
        ? projects.map(p => `<div class="dash-type-item">${esc(p.projectCode || p.name || p.title || p.id || '—')}</div>`).join('')
        : '<div class="dash-type-empty">لا توجد مشاريع</div>';
      return `
        <div class="dash-type-column clickable" onclick="openProjectsByType('${k}')">
          <div class="dash-type-header">
            <span class="dash-type-icon">${info.icon}</span>
            <span class="dash-type-label">${info.ar}</span>
          </div>
          <div class="dash-type-list">${itemsHtml}</div>
          <div class="dash-type-summary">
            <div><span>المشاريع</span><strong>${totalByType}</strong></div>
            <div><span>مكتملة</span><strong>${completedByType}</strong></div>
            <div><span>منتهية</span><strong>${finishedByType}</strong></div>
          </div>
        </div>`;
    })
    .join('') + '</div>';

  const inProgressOrPending = P.filter(p => p.status==='inprog' || p.status==='waiting').length;
  const summaryCardsHtml = `
    <div class="dash-summary-grid">
      <div class="dash-summary-card">
        <div class="dash-summary-label"><span>Implementation</span><span>تنفيذ</span></div>
        <div class="dash-summary-val">${P.filter(p => p.taskTypeKey==='exec').length}</div>
      </div>
      <div class="dash-summary-card">
        <div class="dash-summary-label"><span>Design</span><span>تصميم</span></div>
        <div class="dash-summary-val">${P.filter(p => p.taskTypeKey==='design').length}</div>
      </div>
      <div class="dash-summary-card">
        <div class="dash-summary-label"><span>Supervision</span><span>إشراف</span></div>
        <div class="dash-summary-val">${P.filter(p => p.taskTypeKey==='super').length}</div>
      </div>
      <div class="dash-summary-card">
        <div class="dash-summary-label"><span>Number of Projects</span><span>عدد المشاريع</span></div>
        <div class="dash-summary-val">${total}</div>
      </div>
      <div class="dash-summary-card">
        <div class="dash-summary-label"><span>Completed Projects</span><span>المشاريع المكتملة</span></div>
        <div class="dash-summary-val">${done}</div>
      </div>
      <div class="dash-summary-card">
        <div class="dash-summary-label"><span>In Progress / Pending</span><span>قيد التنفيذ أو موقوفة</span></div>
        <div class="dash-summary-val">${inProgressOrPending}</div>
      </div>
    </div>`;
  document.getElementById('dash-type-chart').innerHTML =
    (chartHtml || '<div class="empty"><i class="ti ti-chart-bar"></i><p>لا توجد بيانات</p></div>') + summaryCardsHtml;

  // Recent activity
  const recent = [...P].sort((a,b)=>b.createdAt-a.createdAt).slice(0,5);
  let actHtml = '';
  for(const p of recent) {
    const c = STATE.clients.find(c=>c.id===p.clientId);
    const t = TYPES[p.taskTypeKey];
    actHtml += `<div style="display:flex;align-items:center;gap:10px;padding:10px 16px;border-bottom:1px solid var(--border);">
      <span style="font-size:18px;">${t?.icon||'📌'}</span>
      <div style="flex:1;min-width:0;">
        <div style="font-size:12.5px;font-weight:600;white-space:nowrap;overflow:hidden;text-overflow:ellipsis;">${esc(p.projectCode)} — ${esc(c?.name||'—')}</div>
        <div style="font-size:11px;color:var(--text3);">${fmtDate(p.createdAt)}</div>
      </div>
      <span class="badge ${STATUS[p.status]?.badge||''}" style="font-size:10px;">${STATUS[p.status]?.ar||p.status}</span>
    </div>`;
  }
  document.getElementById('dash-activity').innerHTML = actHtml || '<div class="empty"><i class="ti ti-clock"></i><p>لا نشاطات</p></div>';

  // Recent projects table
  const tbody = document.querySelector('#dash-recent-tbl tbody');
  if(!tbody) return;
  if(!recent.length) { tbody.innerHTML='<tr><td colspan="6" style="text-align:center;color:var(--text3);padding:30px;">لا توجد مشاريع</td></tr>'; return; }
  tbody.innerHTML = recent.map(p => {
    const c = STATE.clients.find(cl=>cl.id===p.clientId);
    const e = STATE.engineers.find(en=>en.id===p.engineerId);
    const t = TYPES[p.taskTypeKey];
    return `<tr>
      <td><strong>${esc(p.projectCode)}</strong></td>
      <td>${esc(c?.name||'—')}</td>
      <td><span class="badge ${t?.badge}">${t?.icon} ${t?.ar}</span></td>
      <td>${esc(e?.name||'—')}</td>
      <td><span class="badge ${STATUS[p.status]?.badge}">${STATUS[p.status]?.ar}</span></td>
      <td>${p.deliveryDate||'—'}</td>
    </tr>`;
  }).join('');
  if(typeof renderDashRecentLogs==='function') renderDashRecentLogs();
}

// ══════════════════════════════════════════════════════════════════
// CLIENTS
// ══════════════════════════════════════════════════════════════════
function renderClients() {
  // Engineers cannot access clients
  if(CU?.role === 'engineer') {
    const g=document.getElementById('clients-grid');
    if(g) g.innerHTML='<div class="empty"><i class="ti ti-lock"></i><p>ليس لديك صلاحية للوصول إلى بيانات العملاء</p></div>';
    return;
  }
  const q = document.getElementById('client-search')?.value.toLowerCase()||'';
  const addBtn = document.getElementById('clients-add-btn');
  if(addBtn) addBtn.style.display = (CU?.role==='manager')?'flex':'none';
  let list = STATE.clients;
  if(q) list = list.filter(c=>c.name.toLowerCase().includes(q)||String(c.clientCode).includes(q));
  const grid = document.getElementById('clients-grid');
  if(!grid) return;
  // Ensure STATE.reports is always an array
  if(!Array.isArray(STATE.reports)) STATE.reports = [];
  if(!list.length) { grid.innerHTML='<div class="empty" style="grid-column:1/-1;"><i class="ti ti-users"></i><p>لا يوجد عملاء</p></div>'; return; }
  grid.innerHTML = list.map(c => {
    const cProjects = STATE.projects.filter(p=>p.clientId===c.id);
    const fin = c.finance||{totalAmount:0,payments:[]};
    const paid = (fin.payments||[]).filter(p=>p.status==='paid').reduce((s,p)=>s+(p.amount||0),0);
    return `<div class="entity-card">
      <div class="ec-top">
        <div>
          <div class="ec-name">${esc(c.name)}</div>
          <div class="ec-code">${esc(c.clientCode)}</div>
        </div>
        ${CU.role==='manager'?`<div class="act-row">
          <button class="icon-btn edit" onclick="editClient(${c.id})" title="تعديل"><i class="ti ti-edit"></i> تعديل</button>
          <button class="icon-btn del" onclick="deleteClient(${c.id})" title="حذف"><i class="ti ti-trash"></i> حذف</button>
        </div>`:''}
      </div>
      <div style="font-size:12px;color:var(--text3);margin-bottom:6px;display:flex;flex-direction:column;gap:3px;">
        ${c.phone?`<div><i class="ti ti-phone" style="font-size:12px;margin-left:4px;"></i>${esc(c.phone)}</div>`:''}
        ${c.whatsapp&&c.whatsapp!==c.phone?`<div><i class="ti ti-brand-whatsapp" style="font-size:12px;margin-left:4px;color:#25D366;"></i>${esc(c.whatsapp)}</div>`:''}
        ${c.email?`<div><i class="ti ti-mail" style="font-size:12px;margin-left:4px;"></i>${esc(c.email)}</div>`:''}
        ${c.address?`<div><i class="ti ti-map-pin" style="font-size:12px;margin-left:4px;"></i>${esc(c.address)}</div>`:''}
      </div>
      <div class="ec-meta">
        <div class="ec-meta-row"><span class="ec-meta-key">المشاريع</span><span class="ec-meta-val">${cProjects.length}</span></div>
        <div class="ec-meta-row"><span class="ec-meta-key">إجمالي العقود</span><span class="ec-meta-val">${fmt(fin.totalAmount||0, fin.currency||'USD')}</span></div>
        <div class="ec-meta-row"><span class="ec-meta-key">المدفوع</span><span class="ec-meta-val" style="color:var(--green);">${fmt(paid, fin.currency||'USD')}</span></div>
      </div>
    </div>`;
  }).join('');
}

async function deleteClient(id) {
  if(!confirm('حذف العميل وجميع مشاريعه؟')) return;
  const removedProjects = STATE.projects.filter(p => p.clientId===id);
  STATE.projects = STATE.projects.filter(p => p.clientId!==id);
  for(const p of removedProjects) await dbDelete('projects', p.id);
  STATE.clients = STATE.clients.filter(c => c.id!==id);
  await dbDelete('clients', id);
  renderClients(); updateBadges();
  toast('تم حذف العميل');
}

let CLIENT_EDIT_ID = null;

function openAddClient() {
  CLIENT_EDIT_ID = null;
  document.getElementById('client-modal-title').textContent = 'إضافة عميل جديد';
  document.getElementById('client-modal-code').textContent = '';
  document.getElementById('client-name').value      = '';
  document.getElementById('client-code-display').value = 'CLIENT #' + String(STATE.clients.length + 1).padStart(3,'0');
  document.getElementById('client-phone').value     = '';
  document.getElementById('client-whatsapp').value  = '';
  document.getElementById('client-email').value     = '';
  document.getElementById('client-address').value   = '';
  document.getElementById('client-notes').value     = '';
  document.getElementById('client-overlay').classList.add('open');
  setTimeout(() => document.getElementById('client-name').focus(), 100);
}

function editClient(id) {
  CLIENT_EDIT_ID = id;
  const c = STATE.clients.find(cl => cl.id === id);
  if (!c) return;
  document.getElementById('client-modal-title').textContent = 'تعديل بيانات العميل';
  document.getElementById('client-modal-code').textContent  = c.clientCode;
  document.getElementById('client-name').value      = c.name     || '';
  document.getElementById('client-code-display').value = c.clientCode || '';
  document.getElementById('client-phone').value     = c.phone    || '';
  document.getElementById('client-whatsapp').value  = c.whatsapp || '';
  document.getElementById('client-email').value     = c.email    || '';
  document.getElementById('client-address').value   = c.address  || '';
  document.getElementById('client-notes').value     = c.notes    || '';
  document.getElementById('client-overlay').classList.add('open');
  setTimeout(() => document.getElementById('client-name').focus(), 100);
}

function closeClientModal() {
  document.getElementById('client-overlay').classList.remove('open');
  CLIENT_EDIT_ID = null;
}

async function saveClient() {
  const name  = document.getElementById('client-name').value.trim();
  const phone = document.getElementById('client-phone').value.trim();
  if (!name)  { toast('⚠ أدخل اسم العميل');  document.getElementById('client-name').focus();  return; }
  if (!phone) { toast('⚠ أدخل رقم الهاتف'); document.getElementById('client-phone').focus(); return; }

  if (CLIENT_EDIT_ID) {
    // ── Edit existing client ─────────────────────────────────────
    const c = STATE.clients.find(cl => cl.id === CLIENT_EDIT_ID);
    if (!c) return;
    c.name      = name;
    c.phone     = phone;
    c.whatsapp  = document.getElementById('client-whatsapp').value.trim();
    c.email     = document.getElementById('client-email').value.trim();
    c.address   = document.getElementById('client-address').value.trim();
    c.notes     = document.getElementById('client-notes').value.trim();
    c.updatedAt = Date.now();
    await dbPut('clients', c);
    closeClientModal();
    renderClients();
    toast('✓ تم تحديث بيانات العميل');
  } else {
    // ── Add new client ───────────────────────────────────────────
    if (STATE.clients.find(c => c.name === name)) {
      toast('⚠ يوجد عميل بنفس الاسم مسبقاً'); return;
    }
    const newClient = {
      id:          Date.now(),
      clientCode:  'CLIENT #' + String(STATE.clients.length + 1).padStart(3,'0'),
      name,
      phone,
      whatsapp:    document.getElementById('client-whatsapp').value.trim(),
      email:       document.getElementById('client-email').value.trim(),
      address:     document.getElementById('client-address').value.trim(),
      notes:       document.getElementById('client-notes').value.trim(),
      finance:     { totalAmount: 0, payments: [] },
      createdAt:   Date.now()
    };
    await dbPut('clients', newClient);
    STATE.clients.push(newClient);
    closeClientModal();
    renderClients();
    renderDashboard();
    updateBadges();
    toast('✓ تم إضافة العميل — ' + name);
  }
}

// ══════════════════════════════════════════════════════════════════
// PROJECTS
// ══════════════════════════════════════════════════════════════════
function openProjectsByType(type) {
  const typeFilter = document.getElementById('proj-filter-type');
  if(typeFilter) {
    typeFilter.value = type;
  }
  sw('projects', document.querySelector('.ni[data-view=projects]'));
}

function renderProjects() {
  const q = (document.getElementById('proj-search')?.value||'').toLowerCase();
  const ft = document.getElementById('proj-filter-type')?.value||'';
  const fs = document.getElementById('proj-filter-status')?.value||'';
  const fe = document.getElementById('proj-filter-eng')?.value||'';
  const engSel = document.getElementById('proj-filter-eng');
  if(engSel && engSel.options.length<=1) {
    STATE.engineers.forEach(e => { const o=document.createElement('option'); o.value=e.id; o.textContent=e.name; engSel.appendChild(o); });
  }

  let list = STATE.projects;
  if(q) list=list.filter(p=>p.projectCode?.toLowerCase().includes(q)||p.description?.toLowerCase().includes(q)||(STATE.clients.find(c=>c.id===p.clientId)?.name||'').toLowerCase().includes(q));
  if(ft) list=list.filter(p=>p.taskTypeKey===ft);
  if(fs) list=list.filter(p=>p.status===fs);
  if(fe) list=list.filter(p=>String(p.engineerId)===fe);

  const tbody = document.getElementById('projects-tbody');
  if(!tbody) return;
  if(!list.length) { tbody.innerHTML='<tr><td colspan="10" style="text-align:center;color:var(--text3);padding:30px;">لا توجد مشاريع مطابقة</td></tr>'; return; }
  tbody.innerHTML = list.map(p => {
    const c = STATE.clients.find(cl=>cl.id===p.clientId);
    const e = STATE.engineers.find(en=>en.id===p.engineerId);
    const t = TYPES[p.taskTypeKey];
    const s = STATUS[p.status];
    const pr = PRI[p.priority];
    const prog = p.progress||0;
    const delBtnHtml = CU.role==='manager'?`<button class="proj-btn proj-btn-del" onclick="deleteProject(${p.id})"><i class="ti ti-trash"></i> حذف</button>`:'';
    return `<tr>
      <td><strong style="font-family:monospace;">${esc(p.projectCode)}</strong></td>
      <td>${esc(c?.name||'—')}</td>
      <td><span class="badge ${t?.badge}">${t?.icon} ${t?.ar}</span></td>
      <td style="max-width:180px;white-space:nowrap;overflow:hidden;text-overflow:ellipsis;" title="${esc(p.description)}">${esc(p.description||'—')}</td>
      <td>${esc(e?.name||'—')}</td>
      <td><span class="badge ${pr?.badge}">${pr?.ar}</span></td>
      <td><span class="badge ${s?.badge}">${s?.ar}</span></td>
      <td>${p.deliveryDate||'—'}</td>
      <td><div style="display:flex;align-items:center;gap:6px;"><div class="prog-bar" style="width:60px;"><div class="prog-fill" style="width:${prog}%;"></div></div><span style="font-size:11px;">${prog}%</span></div></td>
      <td style="min-width:230px;">
        <div class="proj-action-row">
          <button class="proj-btn proj-btn-edit" onclick="openEditWO(${p.id})">
            <i class="ti ti-edit"></i> تعديل
          </button>
          <button class="proj-btn proj-btn-follow" onclick="openFollowup(${p.id})">
            <i class="ti ti-list-check"></i> متابعة
          </button>
          ${delBtnHtml}
        </div>
      </td>
    </tr>`;
  }).join('');
}

async function deleteProject(id) {
  if(!confirm('حذف هذا المشروع؟')) return;
  STATE.projects = STATE.projects.filter(p=>p.id!==id);
  await dbDelete('projects', id);
  renderProjects(); renderDashboard(); updateBadges();
  logActivity('حذف مشروع', p.projectCode);
  toast('تم حذف المشروع');
}

// ══════════════════════════════════════════════════════════════════
// ENGINEER TASKS
// ══════════════════════════════════════════════════════════════════
function renderEngTasks() {
  const fs = document.getElementById('et-filter-status')?.value||'';
  const fp = document.getElementById('et-filter-pri')?.value||'';
  let list = STATE.projects;
  if(CU.role==='engineer') list = list.filter(p=>{
    const eng = STATE.engineers.find(e=>e.name===CU.name||e.username===CU.username);
    return eng?p.engineerId===eng.id:false;
  });
  if(fs) list=list.filter(p=>p.status===fs);
  if(fp) list=list.filter(p=>p.priority===fp);

  const el = document.getElementById('eng-tasks-list');
  if(!el) return;
  if(!list.length) {
    el.innerHTML='<div class="empty"><i class="ti ti-clipboard"></i><p>لا توجد مهام مسندة</p></div>';
    return;
  }
  el.innerHTML = list.map(p=>{
    const c = STATE.clients.find(cl=>cl.id===p.clientId);
    const t = TYPES[p.taskTypeKey];
    const s = STATUS[p.status];
    const pr = PRI[p.priority];
    const prog = p.progress||0;
    const canUpdate = CU.role==='engineer'||CU.role==='manager';
    return `<div class="eng-task-card">
      <div class="etc-header">
        <span class="etc-code">${esc(p.projectCode)}</span>
        <span class="etc-name">${esc(p.description||'—')}</span>
        <span class="badge ${s?.badge}">${s?.ar}</span>
        <span class="badge ${pr?.badge}">${pr?.ar}</span>
        ${canUpdate?`<button class="tbtn" onclick="openEngUpd(${p.id})" style="padding:5px 10px;font-size:12px;"><i class="ti ti-edit"></i> تحديث</button>`:''}
      </div>
      <div class="etc-body">
        <div class="etc-field"><div class="etc-field-lbl">العميل</div><div class="etc-field-val">${esc(c?.name||'—')}</div></div>
        <div class="etc-field"><div class="etc-field-lbl">النوع</div><div class="etc-field-val"><span class="badge ${t?.badge}">${t?.icon} ${t?.ar}</span></div></div>
        <div class="etc-field"><div class="etc-field-lbl">تاريخ التسليم</div><div class="etc-field-val">${p.deliveryDate||'—'}</div></div>
        <div class="etc-field"><div class="etc-field-lbl">تاريخ الاستلام</div><div class="etc-field-val">${p.receivedDate||'—'}</div></div>
      </div>
      <div class="etc-progress">
        <div class="etc-prog-top"><span style="color:var(--text3);font-size:12px;">الإنجاز</span><span style="font-size:12px;font-weight:700;">${prog}%</span></div>
        <div class="prog-bar" style="height:8px;"><div class="prog-fill" style="width:${prog}%;"></div></div>
      </div>
      ${p.engineerNotes?`<div style="margin-top:10px;font-size:11.5px;color:var(--text2);background:var(--surface2);padding:8px 10px;border-radius:var(--radius-sm);"><strong>ملاحظات:</strong> ${esc(p.engineerNotes)}</div>`:''}
    </div>`;
  }).join('');
}

function openEngUpd(id) {
  ENG_UPD_ID = id;
  const p = STATE.projects.find(pr=>pr.id===id);
  if(!p) return;
  document.getElementById('eu-subtitle').textContent = p.projectCode + ' — ' + (p.description||'');
  document.getElementById('eu-status').value = p.status;
  document.getElementById('eu-progress').value = p.progress||0;
  document.getElementById('eu-notes').value = p.engineerNotes||'';
  document.getElementById('eng-upd-overlay').classList.add('open');
}
function closeEngUpd() { document.getElementById('eng-upd-overlay').classList.remove('open'); }

async function saveEngUpd() {
  const p = STATE.projects.find(pr=>pr.id===ENG_UPD_ID);
  if(!p) return;
  p.status = document.getElementById('eu-status').value;
  p.progress = parseInt(document.getElementById('eu-progress').value)||0;
  p.engineerNotes = document.getElementById('eu-notes').value.trim();
  p.updatedAt = Date.now();
  await dbPut('projects', p);
  closeEngUpd();
  renderEngTasks(); renderDashboard(); updateBadges();
  toast('✓ تم تحديث المهمة');
}

// ══════════════════════════════════════════════════════════════════
// FINANCE v2 — Full financial management system
// ══════════════════════════════════════════════════════════════════

// Active project/client in finance modals
let PFIN_PROJECT_ID = null;
let PFIN_TAB = 'all';
let PAY_RECEIPT_DATA = null;   // base64 of payment receipt
let EXP_RECEIPT_DATA = null;   // base64 of expense receipt
let CFIN_CLIENT_ID = null;
let FIN_TAB = 'clients'; // 'clients' | 'ws' | 'wk'
let FIN_PAY_PROJ_ID = null; // project id for finance-section payments
let FIN_PAY_ENT_ID  = null; // entity id (workshop or worker)
let FIN_PAY_ENT_TYPE = null; // 'ws' | 'wk'

// Expense category config
const EXP_CATS = {
  materials:  { ar: 'مواد', icon: '🧱' },
  labor:      { ar: 'أجور عمال', icon: '👷' },
  municipal:  { ar: 'رسوم بلدية', icon: '🏛️' },
  license:    { ar: 'رسوم تراخيص', icon: '📜' },
  transport:  { ar: 'نقل ومواصلات', icon: '🚗' },
  sitevisit:  { ar: 'زيارات ميدانية', icon: '📍' },
  admin:      { ar: 'مصاريف إدارية', icon: '📊' },
  other:      { ar: 'مصاريف أخرى', icon: '📦' }
};

// ── Helpers ──
function getProjFin(p) {
  if (!p.fin2) p.fin2 = {
    contractAmount: p.totalAmount || 0,
    currency:       p.currency || 'USD',
    payments:  [],
    expenses:  []
  };
  if (!p.fin2.payments) p.fin2.payments = [];
  if (!p.fin2.expenses) p.fin2.expenses = [];
  if (!p.fin2.contractAmount && p.totalAmount) p.fin2.contractAmount = p.totalAmount;
  if (!p.fin2.currency) p.fin2.currency = p.currency || 'USD';
  return p.fin2;
}

function calcProjTotals(p) {
  const fin = getProjFin(p);
  const cur = fin.currency || p.currency || 'USD';
  const contractAmt = fin.contractAmount || 0;
  const paid    = fin.payments.reduce((s,x) => s + (x.amount||0), 0);
  let expenses  = fin.expenses.reduce((s,x) => s + (x.amount||0), 0);
  // Exec/Super: auto-include workforce costs as expenses
  if (isExecType(p) && p.workforce) {
    const wft = calcWorkforceTotals(p);
    expenses += wft.total; // workshops + workers total
  }
  const remaining = contractAmt - paid;
  const netProfit = paid - expenses;
  return { contractAmt, paid, expenses, remaining, netProfit, cur, sym: CURRENCY_SYMBOL[cur]||cur };
}

// toSAR removed

function fmt(amount, currency) {
  const sym = CURRENCY_SYMBOL[currency] || currency || '';
  return (amount||0).toLocaleString() + ' ' + sym;
}

function calcClientTotals(clientId) {
  // Convert all to USD for unified global display (approximate)
  const projs = STATE.projects.filter(p=>p.clientId===clientId);
  let contractUSD=0, paidUSD=0, expUSD=0;
  projs.forEach(p=>{
    const t = calcProjTotals(p);
    contractUSD += toUSD(t.contractAmt, t.cur);
    paidUSD     += toUSD(t.paid,        t.cur);
    expUSD      += toUSD(t.expenses,    t.cur);
  });
  return {
    contractAmt: contractUSD, paid: paidUSD, expenses: expUSD,
    remaining: contractUSD - paidUSD, netProfit: paidUSD - expUSD,
    cur: 'USD', sym: '$', projCount: projs.length
  };
}

// ── Finance tab switch ──────────────────────────────────────────
function setFinTab(tab) {
  FIN_TAB = tab;
  ['clients','ws','wk'].forEach(t => {
    document.getElementById('fin-tab-'+t)?.classList.toggle('on', t===tab);
  });
  const showSearch = true; // search always visible
  document.getElementById('finance-grid')?.style.setProperty('display', tab==='clients'?'':'none');
  document.getElementById('fin-ws-grid')?.style.setProperty('display',  tab==='ws'?'':'none');
  document.getElementById('fin-wk-grid')?.style.setProperty('display',  tab==='wk'?'':'none');
  renderFinance();
}

// ── Helper: collect all exec/super workshops from all projects ──
function getAllWorkshops() {
  const res = [];
  STATE.projects.filter(p=>isExecType(p)).forEach(p=>{
    const c   = STATE.clients.find(cl=>cl.id===p.clientId);
    const fin = getProjFin(p);
    const cur = fin.currency || p.currency || 'USD';
    (p.workforce?.workshops||[]).forEach(s=>{
      res.push({ proj:p, client:c, ws:s, cur });
    });
  });
  return res;
}
function getAllWorkers() {
  const res = [];
  STATE.projects.filter(p=>isExecType(p)).forEach(p=>{
    const c   = STATE.clients.find(cl=>cl.id===p.clientId);
    const fin = getProjFin(p);
    const cur = fin.currency || p.currency || 'USD';
    (p.workforce?.workers||[]).forEach(w=>{
      res.push({ proj:p, client:c, wk:w, cur });
    });
  });
  return res;
}

// ── Payment type labels ──────────────────────────────────────────
function payTypeLabel(t) {
  return {advance:'مقدمة', milestone:'مرحلية', final:'نهائية', partial:'جزئية'}[t] || t || 'دفعة';
}
function payMethodLabel(m) {
  return {cash:'نقداً', transfer:'تحويل', cheque:'شيك'}[m] || m || '';
}

// ── Open payment form (inline inside card) ───────────────────────
function finOpenPay(projId, entId, entType) {
  FIN_PAY_PROJ_ID  = projId;
  FIN_PAY_ENT_ID   = entId;
  FIN_PAY_ENT_TYPE = entType;
  // Hide all other open forms first
  document.querySelectorAll('.fin-pay-form').forEach(f=>f.classList.remove('show'));
  const formEl = document.getElementById(`fin-pf-${entId}`);
  if (formEl) {
    formEl.classList.add('show');
    formEl.querySelector('.fin-pf-amount')?.focus();
  }
}
function finClosePay(entId) {
  document.getElementById(`fin-pf-${entId}`)?.classList.remove('show');
}

async function finSavePay(entId) {
  const form   = document.getElementById(`fin-pf-${entId}`);
  if (!form) return;
  const amount = parseFloat(form.querySelector('.fin-pf-amount').value) || 0;
  const date   = form.querySelector('.fin-pf-date').value;
  const method = form.querySelector('.fin-pf-method').value;
  const ref    = form.querySelector('.fin-pf-ref').value.trim();
  const notes  = form.querySelector('.fin-pf-notes').value.trim();
  const ptype  = form.querySelector('.fin-pf-type')?.value || 'partial';

  // Validation
  if (!amount || amount <= 0) { toast('⚠ أدخل مبلغًا صحيحًا'); return; }
  if (!date)                  { toast('⚠ أدخل التاريخ'); return; }

  const p = STATE.projects.find(x=>x.id===FIN_PAY_PROJ_ID);
  if (!p) return;

  let entity, total, paid;
  if (FIN_PAY_ENT_TYPE === 'ws') {
    entity = (p.workforce?.workshops||[]).find(x=>x.id===entId);
    if (!entity) return;
    if (!entity.payments) entity.payments = [];
    total = spTotal(entity);
    paid  = spPaid(entity);
  } else {
    entity = (p.workforce?.workers||[]).find(x=>x.id===entId);
    if (!entity) return;
    if (!entity.payments) entity.payments = [];
    total = wkTotal(entity);
    paid  = wkPaid(entity);
  }

  const remaining = total - paid;
  if (amount > remaining + 0.01) {
    toast(`⚠ المبلغ (${fmt(amount, getProjFin(p).currency||'USD')}) يتجاوز المتبقي (${fmt(remaining, getProjFin(p).currency||'USD')})`);
    return;
  }

  entity.payments.push({
    id: fuUID('fp'), amount, date, type: ptype,
    method, ref, notes, createdAt: Date.now()
  });
  p.updatedAt = Date.now();
  await dbPut('projects', p);

  // Reset form
  form.querySelector('.fin-pf-amount').value = '';
  form.querySelector('.fin-pf-ref').value    = '';
  form.querySelector('.fin-pf-notes').value  = '';
  form.classList.remove('show');

  // Reactive refresh
  renderFinance();
  if (document.getElementById('pfin-overlay')?.classList.contains('open') && PFIN_PROJECT_ID===p.id)
    renderProjKpis();
  toast(`✓ تم تسجيل الدفعة`);
}

async function finDeletePay(projId, entId, entType, payId) {
  if (!confirm('حذف هذه الدفعة؟')) return;
  const p = STATE.projects.find(x=>x.id===projId); if(!p) return;
  const arr = entType==='ws'
    ? (p.workforce?.workshops||[]).find(x=>x.id===entId)
    : (p.workforce?.workers||[]).find(x=>x.id===entId);
  if (!arr) return;
  arr.payments = (arr.payments||[]).filter(x=>x.id!==payId);
  await dbPut('projects',p);
  renderFinance();
  toast('تم حذف الدفعة');
}

// ── Build payment form HTML ──────────────────────────────────────
function buildPayForm(entId, entType, cur) {
  const typeOpts = entType==='ws'
    ? `<option value="advance">💵 مقدمة</option>
       <option value="milestone">🏁 مرحلية</option>
       <option value="final">✅ نهائية</option>`
    : `<option value="partial">💰 جزئية</option>
       <option value="final">✅ نهائية</option>`;
  return `<div class="fin-pay-form" id="fin-pf-${entId}">
    <div style="font-size:12px;font-weight:700;color:var(--green);margin-bottom:10px;">
      <i class="ti ti-cash" style="vertical-align:-2px;margin-left:4px;"></i>تسجيل دفعة جديدة
    </div>
    <div class="frow3" style="gap:10px;">
      <div class="fg">
        <label style="font-size:11px;">نوع الدفعة</label>
        <select class="fi fin-pf-type" style="font-size:12px;">${typeOpts}</select>
      </div>
      <div class="fg">
        <label style="font-size:11px;">المبلغ <span class="req">*</span></label>
        <input class="fi fin-pf-amount" type="number" min="0.01" step="0.01"
          placeholder="0" style="font-size:13px;font-weight:700;color:var(--accent);">
      </div>
      <div class="fg">
        <label style="font-size:11px;">التاريخ <span class="req">*</span></label>
        <input class="fi fin-pf-date" type="date"
          value="${new Date().toISOString().split('T')[0]}" style="font-size:12px;">
      </div>
    </div>
    <div class="frow" style="gap:10px;margin-top:8px;">
      <div class="fg">
        <label style="font-size:11px;">طريقة الدفع</label>
        <select class="fi fin-pf-method" style="font-size:12px;">
          <option value="cash">نقداً</option>
          <option value="transfer">تحويل بنكي</option>
          <option value="cheque">شيك</option>
          <option value="">أخرى</option>
        </select>
      </div>
      <div class="fg">
        <label style="font-size:11px;">المرجع</label>
        <input class="fi fin-pf-ref" placeholder="رقم العملية..." style="font-size:12px;">
      </div>
    </div>
    <div class="fg" style="margin-top:8px;">
      <label style="font-size:11px;">ملاحظات</label>
      <input class="fi fin-pf-notes" placeholder="(اختياري)" style="font-size:12px;">
    </div>
    <div style="display:flex;gap:8px;margin-top:10px;">
      <button class="btn-save" style="background:var(--green);font-size:12.5px;padding:8px 18px;"
        onclick="finSavePay('${entId}')">
        <i class="ti ti-check" style="vertical-align:-2px;margin-left:4px;"></i>حفظ الدفعة
      </button>
      <button class="btn-cancel" style="font-size:12px;"
        onclick="finClosePay('${entId}')">إلغاء</button>
    </div>
  </div>`;
}

// ── Render Workshops financial section ───────────────────────────
function renderFinanceWorkshops() {
  const grid = document.getElementById('fin-ws-grid');
  if (!grid) return;
  const q = (document.getElementById('fin2-search')?.value||'').toLowerCase();

  // Get all exec/super projects that have workshops
  let projects = STATE.projects.filter(p => isExecType(p) && (p.workforce?.workshops||[]).length > 0);
  if(q) projects = projects.filter(p => {
    const c = STATE.clients.find(cl=>cl.id===p.clientId);
    return (p.projectCode||'').toLowerCase().includes(q) ||
           (p.description||'').toLowerCase().includes(q) ||
           (c?.name||'').toLowerCase().includes(q) ||
           (p.workforce?.workshops||[]).some(w=>(w.name||'').toLowerCase().includes(q));
  });

  if(!projects.length) {
    grid.innerHTML = `<div class="empty"><i class="ti ti-building-warehouse"></i><p>لا توجد ورشات في مشاريع التنفيذ والإشراف</p></div>`;
    return;
  }

  // Global KPIs (all projects)
  let gWsTotal=0, gWsPaid=0, gWkCost=0, gWkPaid=0, gMatCost=0, gEqpCost=0;
  projects.forEach(p => {
    const fin = getProjFin(p);
    const wft = calcWorkforceTotals(p);
    gWsTotal += wft.wsContract; gWsPaid += wft.wsPaid;
    gWkCost  += wft.wkCost;     gWkPaid += wft.wkPaidAmt;
    gMatCost += (fin.materials||[]).reduce((s,m)=>s+(m.qty||0)*(m.price||0),0);
    gEqpCost += (fin.equipment||[]).reduce((s,e)=>s+(e.dailyRate||0)*(e.days||0),0);
  });
  const gTotal = gWsTotal + gWkCost + gMatCost + gEqpCost;
  const gPaid  = gWsPaid  + gWkPaid;

  const globalSummary = `
    <div style="display:grid;grid-template-columns:repeat(4,1fr);gap:10px;margin-bottom:20px;">
      <div class="fin-ws-card" style="border-top:3px solid var(--blue);">
        <div style="padding:12px 16px;">
          <div style="font-size:10px;color:var(--text3);margin-bottom:3px;">إجمالي الورشات</div>
          <div style="font-size:17px;font-weight:700;">${fmt(gWsTotal,'USD')}</div>
          <div style="font-size:11px;color:var(--green);">مدفوع: ${fmt(gWsPaid,'USD')}</div>
        </div>
      </div>
      <div class="fin-ws-card" style="border-top:3px solid var(--amber);">
        <div style="padding:12px 16px;">
          <div style="font-size:10px;color:var(--text3);margin-bottom:3px;">إجمالي العمال</div>
          <div style="font-size:17px;font-weight:700;">${fmt(gWkCost,'USD')}</div>
          <div style="font-size:11px;color:var(--green);">مدفوع: ${fmt(gWkPaid,'USD')}</div>
        </div>
      </div>
      <div class="fin-ws-card" style="border-top:3px solid var(--project-c,var(--accent));">
        <div style="padding:12px 16px;">
          <div style="font-size:10px;color:var(--text3);margin-bottom:3px;">مواد + معدات</div>
          <div style="font-size:17px;font-weight:700;">${fmt(gMatCost+gEqpCost,'USD')}</div>
          <div style="font-size:11px;color:var(--text3);">مواد: ${fmt(gMatCost,'USD')}</div>
        </div>
      </div>
      <div class="fin-ws-card" style="border-top:3px solid ${gTotal>gPaid?'var(--red)':'var(--green)'};">
        <div style="padding:12px 16px;">
          <div style="font-size:10px;color:var(--text3);margin-bottom:3px;">إجمالي الالتزامات</div>
          <div style="font-size:17px;font-weight:700;">${fmt(gTotal,'USD')}</div>
          <div style="font-size:11px;color:${gTotal>gPaid?'var(--red)':'var(--green)'};">متبقي: ${fmt(gTotal-gPaid,'USD')}</div>
        </div>
      </div>
    </div>`;

  // Project cards
  const projectCards = projects.map(p => {
    const c   = STATE.clients.find(cl=>cl.id===p.clientId);
    const fin = getProjFin(p);
    const cur = fin.currency || p.currency || 'USD';
    const wks = p.workforce?.workshops || [];
    const wkrs= p.workforce?.workers   || [];
    const typeCfg = TYPES[p.taskTypeKey]||{};
    const stCfg   = STATUS[p.status]||{ar:p.status,badge:''};

    // Per-project financial summary
    const wft      = calcWorkforceTotals(p);
    const matCost  = (fin.materials||[]).reduce((s,m)=>s+(m.qty||0)*(m.price||0),0);
    const eqpCost  = (fin.equipment||[]).reduce((s,e)=>s+(e.dailyRate||0)*(e.days||0),0);
    const expCost  = (fin.expenses||[]).reduce((s,x)=>s+(x.amount||0),0);
    const totOblig = wft.wsContract + wft.wkCost + matCost + eqpCost + expCost;
    const totPaid  = wft.wsPaid + wft.wkPaidAmt;
    const netOblig = totOblig - totPaid;

    // Workshop rows
    const wsRows = wks.map(ws => {
      if(!ws.payments) ws.payments=[];
      const wsTotal = spTotal(ws);
      const wsPd    = spPaid(ws);
      const wsRem   = wsTotal - wsPd;
      const pct     = wsTotal ? Math.round(wsPd/wsTotal*100) : 0;
      const prog    = ws.progress||0;
      const progDue = wsTotal * prog / 100;
      const remColor = wsRem>0 ? 'var(--red)' : 'var(--green)';

      // Payment ledger inside expand panel
      let runBal=0;
      const payRows = ws.payments.map((pm,idx)=>{
        runBal += pm.amount||0;
        const remaining = wsTotal - runBal;
        return `<div class="fin-pay-row">
          <span class="fin-pay-num">${idx+1}</span>
          <span class="fin-pay-type">${payTypeLabel(pm.type)}</span>
          <span class="fin-pay-date">${pm.date||'—'}</span>
          <span class="fin-pay-method">${payMethodLabel(pm.method)}</span>
          ${pm.ref?`<span style="font-size:10px;color:var(--text3);">${esc(pm.ref)}</span>`:''}
          <span class="fin-pay-amt">${fmt(pm.amount||0,cur)}</span>
          <span class="fin-pay-rem">متبقي: ${fmt(Math.max(0,remaining),cur)}</span>
          <button class="icon-btn del" style="width:26px;height:26px;"
            onclick="finDeletePay(${p.id},'${ws.id}','ws','${pm.id}')" title="حذف">
            <i class="ti ti-trash" style="font-size:12px;"></i>
          </button>
        </div>`;
      }).join('');

      const isExp = !!WS_EXPANDED[ws.id];

      return `
        <div class="ws-row">
          <!-- Row header (click to expand) -->
          <div class="ws-row-header ${isExp?'expanded':''}" id="wsh-${ws.id}"
            onclick="wsToggleDetail('${ws.id}')">
            <div class="ws-row-left">
              <i class="ti ti-building-warehouse" style="color:var(--accent);font-size:16px;flex-shrink:0;"></i>
              <div>
                <div class="ws-row-name">${esc(ws.name||'ورشة بدون اسم')}</div>
                <div class="ws-row-formula" style="font-size:10.5px;color:var(--text3);">
                  ${ws.qty&&ws.unitPrice ? ws.qty+' '+esc(ws.unit||'')+'× '+fmt(ws.unitPrice,cur)+' = '+fmt(wsTotal,cur) : fmt(wsTotal,cur)}
                  ${ws.item ? ' — '+esc(ws.item) : ''}
                </div>
              </div>
            </div>
            <div class="ws-row-right">
              <div class="ws-row-kpi" style="min-width:70px;text-align:right;">
                <div class="ws-row-kpi-lbl">قيمة العقد</div>
                <div class="ws-row-kpi-val">${fmt(wsTotal,cur)}</div>
              </div>
              <div class="ws-row-kpi" style="min-width:70px;text-align:right;">
                <div class="ws-row-kpi-lbl" style="color:var(--green);">مدفوع</div>
                <div class="ws-row-kpi-val" style="color:var(--green);">${fmt(wsPd,cur)}</div>
              </div>
              <div class="ws-row-kpi" style="min-width:70px;text-align:right;">
                <div class="ws-row-kpi-lbl" style="color:${remColor};">متبقي</div>
                <div class="ws-row-kpi-val" style="color:${remColor};">${wsRem>0?fmt(wsRem,cur):'✓ مسدد'}</div>
              </div>
              <div style="text-align:center;">
                <div style="font-size:9.5px;color:var(--text3);margin-bottom:3px;">إنجاز</div>
                <div class="ws-prog-bar-sm"><div class="ws-prog-fill-sm" style="width:${prog}%;"></div></div>
                <div style="font-size:9.5px;font-weight:700;margin-top:2px;">${prog}%</div>
              </div>
              <i class="ti ti-chevron-down ws-chevron ${isExp?'open':''}" id="wsico-${ws.id}"></i>
            </div>
          </div>

          <!-- Expand panel -->
          <div class="ws-detail-panel ${isExp?'open':''}" id="wsd-${ws.id}">
            <!-- Details grid -->
            <div class="ws-detail-grid">
              <div class="ws-detail-field"><div class="ws-detail-lbl">المسؤول</div><div class="ws-detail-val">${esc(ws.manager||'—')}</div></div>
              <div class="ws-detail-field"><div class="ws-detail-lbl">الهاتف</div><div class="ws-detail-val">${esc(ws.phone||'—')}</div></div>
              <div class="ws-detail-field"><div class="ws-detail-lbl">نوع العمل</div><div class="ws-detail-val">${esc(ws.type||'—')}</div></div>
              <div class="ws-detail-field"><div class="ws-detail-lbl">البند المرتبط</div><div class="ws-detail-val">${esc(ws.item||'—')}</div></div>
              <div class="ws-detail-field"><div class="ws-detail-lbl">الكمية</div><div class="ws-detail-val">${ws.qty||'—'} ${esc(ws.unit||'')}</div></div>
              <div class="ws-detail-field"><div class="ws-detail-lbl">سعر الوحدة</div><div class="ws-detail-val">${fmt(ws.unitPrice||0,cur)}</div></div>
              <div class="ws-detail-field"><div class="ws-detail-lbl">القيمة الإجمالية</div><div class="ws-detail-val" style="color:var(--accent);">${fmt(wsTotal,cur)}</div></div>
              ${prog>0?`<div class="ws-detail-field"><div class="ws-detail-lbl">مستحق مرحلي (${prog}%)</div><div class="ws-detail-val" style="color:var(--amber);">${fmt(progDue,cur)}</div></div>`:''}
            </div>
            <!-- Payment ledger -->
            ${ws.payments.length?`
            <div class="fin-pay-ledger" style="margin-bottom:10px;">
              <div class="fin-pay-ledger-title"><i class="ti ti-list-numbers"></i>سجل الدفعات (${ws.payments.length})</div>
              ${payRows}
            </div>`:''}
            <!-- Add payment form -->
            ${wsRem>0 ? buildPayForm(ws.id,'ws',cur) : '<div style="font-size:12px;color:var(--green);font-weight:700;padding:6px 0;">✅ تم السداد الكامل</div>'}
            ${wsRem>0 ? `<button class="fin-add-pay-btn" style="margin-top:8px;" onclick="finOpenPay(${p.id},'${ws.id}','ws')">
              <i class="ti ti-plus"></i> إضافة دفعة
            </button>` : ''}
            <button class="ws-proj-edit-btn" onclick="printSingleWorkshop(${p.id},'${ws.id}')"
              style="margin-top:10px;background:var(--accent-light);color:var(--accent);border:1px solid var(--accent-mid);">
              <i class="ti ti-printer"></i> طباعة هذه الورشة
            </button>
          </div>
        </div>`;
    }).join('');

    return `
    <div class="ws-proj-card">
      <!-- Project header with financial summary -->
      <div class="ws-proj-header">
        <div class="ws-proj-title">
          <div>
            <div style="display:flex;align-items:center;gap:8px;flex-wrap:wrap;">
              <span class="ws-proj-name" id="wsn-${p.id}">${esc(p.projectCode)} — ${esc(p.description||'مشروع')}</span>
              <input class="ws-proj-name-input" id="wsnInp-${p.id}"
                value="${esc(p.description||'')}" style="display:none;"
                onblur="wsSaveName(${p.id})"
                onkeydown="if(event.key==='Enter')wsSaveName(${p.id});if(event.key==='Escape'){this.style.display='none';document.getElementById('wsn-${p.id}').style.display='';}">
              <button class="ws-proj-edit-btn" onclick="wsEditName(${p.id})">
                <i class="ti ti-pencil"></i> تعديل الاسم
              </button>
              <button class="ws-proj-edit-btn" onclick="printProjectWorkshops(${p.id})"
                style="background:rgba(255,255,255,.2);">
                <i class="ti ti-printer"></i> طباعة المشروع
              </button>
            </div>
            <div class="ws-proj-badges" style="margin-top:5px;">
              <span style="background:rgba(255,255,255,.15);color:#fff;font-size:10px;padding:2px 8px;border-radius:10px;">${typeCfg.icon||''} ${typeCfg.ar||''}</span>
              <span style="background:rgba(255,255,255,.15);color:#fff;font-size:10px;padding:2px 8px;border-radius:10px;">👤 ${esc(c?.name||'—')}</span>
              <span style="background:rgba(255,255,255,.15);color:#fff;font-size:10px;padding:2px 8px;border-radius:10px;">${stCfg.ar}</span>
              <span style="background:rgba(255,255,255,.15);color:#fff;font-size:10px;padding:2px 8px;border-radius:10px;">🏗️ ${wks.length} ورشة</span>
            </div>
          </div>
        </div>
        <!-- Financial summary -->
        <div class="ws-fin-summary">
          <div class="ws-fin-kpi">
            <div class="ws-fin-kpi-lbl">قيمة الورشات</div>
            <div class="ws-fin-kpi-val">${fmt(wft.wsContract,cur)}</div>
            <div style="font-size:9.5px;opacity:.7;">مدفوع: ${fmt(wft.wsPaid,cur)}</div>
          </div>
          <div class="ws-fin-kpi">
            <div class="ws-fin-kpi-lbl">تكلفة العمال</div>
            <div class="ws-fin-kpi-val">${fmt(wft.wkCost,cur)}</div>
            <div style="font-size:9.5px;opacity:.7;">مدفوع: ${fmt(wft.wkPaidAmt,cur)}</div>
          </div>
          <div class="ws-fin-kpi">
            <div class="ws-fin-kpi-lbl">المواد + المعدات</div>
            <div class="ws-fin-kpi-val">${fmt(matCost+eqpCost,cur)}</div>
            <div style="font-size:9.5px;opacity:.7;">مواد: ${fmt(matCost,cur)} | معدات: ${fmt(eqpCost,cur)}</div>
          </div>
          <div class="ws-fin-kpi">
            <div class="ws-fin-kpi-lbl">إجمالي الالتزامات</div>
            <div class="ws-fin-kpi-val">${fmt(totOblig,cur)}</div>
            <div style="font-size:9.5px;opacity:.7;">مصروفات: ${fmt(expCost,cur)}</div>
          </div>
          <div class="ws-fin-kpi">
            <div class="ws-fin-kpi-lbl">صافي المتبقي</div>
            <div class="ws-fin-kpi-val" style="color:${netOblig>0?'#fca5a5':'#86efac'};">${fmt(netOblig,cur)}</div>
            <div style="font-size:9.5px;opacity:.7;">مدفوع: ${fmt(totPaid,cur)}</div>
          </div>
        </div>
      </div>
      <!-- Workshop rows -->
      <div>${wsRows}</div>
    </div>`;
  }).join('');

  grid.innerHTML = globalSummary + projectCards;
}

// ── Render Workers financial section ─────────────────────────────
function renderFinanceWorkers() {
  const grid = document.getElementById('fin-wk-grid');
  if (!grid) return;
  const q    = (document.getElementById('fin2-search')?.value||'').toLowerCase();
  let items  = getAllWorkers();
  if (q) items = items.filter(({proj,client,wk})=>
    (wk.name||'').toLowerCase().includes(q) ||
    (proj.projectCode||'').toLowerCase().includes(q) ||
    (client?.name||'').toLowerCase().includes(q));

  if (!items.length) {
    grid.innerHTML = `<div class="empty"><i class="ti ti-hard-hat"></i><p>لا يوجد عمال في مشاريع التنفيذ والإشراف</p></div>`;
    return;
  }

  let gTotal=0, gPaid=0;
  items.forEach(({wk})=>{ gTotal+=wkTotal(wk); gPaid+=wkPaid(wk); });
  const gRem = gTotal - gPaid;

  let summaryHtml = `<div style="display:grid;grid-template-columns:repeat(3,1fr);gap:12px;margin-bottom:18px;">
    <div class="fin-wk-card" style="border-top:3px solid var(--amber);">
      <div style="padding:14px 18px;">
        <div style="font-size:10px;color:var(--text3);margin-bottom:4px;">إجمالي تكلفة العمال</div>
        <div style="font-size:20px;font-weight:700;">${fmt(gTotal,'USD')}</div>
      </div>
    </div>
    <div class="fin-wk-card" style="border-top:3px solid var(--green);">
      <div style="padding:14px 18px;">
        <div style="font-size:10px;color:var(--green);margin-bottom:4px;">إجمالي المدفوع</div>
        <div style="font-size:20px;font-weight:700;color:var(--green);">${fmt(gPaid,'USD')}</div>
      </div>
    </div>
    <div class="fin-wk-card" style="border-top:3px solid ${gRem>0?'var(--red)':'var(--green)'};">
      <div style="padding:14px 18px;">
        <div style="font-size:10px;color:${gRem>0?'var(--red)':'var(--text3)'};margin-bottom:4px;">المستحق للعمال</div>
        <div style="font-size:20px;font-weight:700;color:${gRem>0?'var(--red)':'var(--green)'};">${gRem>0?fmt(gRem,'USD'):'مسدد ✓'}</div>
      </div>
    </div>
  </div>`;

  let cardsHtml = items.map(({proj,client,wk,cur})=>{
    if (!wk.payments) wk.payments=[];
    const total   = wkTotal(wk);
    const paid    = wkPaid(wk);
    const rem     = total - paid;
    const paidPct = total?Math.round(paid/total*100):0;
    const typeCfg = TYPES[proj.taskTypeKey]||{};

    let runBal=0;
    const payRows = wk.payments.map((pm,idx)=>{
      runBal += pm.amount||0;
      const remaining = total - runBal;
      return `<div class="fin-pay-row">
        <span class="fin-pay-num">${idx+1}</span>
        <span class="fin-pay-type">${payTypeLabel(pm.type)}</span>
        <span class="fin-pay-date">${pm.date||'—'}</span>
        <span class="fin-pay-method">${payMethodLabel(pm.method)}</span>
        <span class="fin-pay-amt">${fmt(pm.amount||0,cur)}</span>
        <span class="fin-pay-rem">متبقي: ${fmt(Math.max(0,remaining),cur)}</span>
        <button class="icon-btn del" style="width:26px;height:26px;"
          onclick="finDeletePay(${proj.id},'${wk.id}','wk','${pm.id}')" title="حذف">
          <i class="ti ti-trash" style="font-size:12px;"></i>
        </button>
      </div>`;
    }).join('');

    return `<div class="fin-wk-card">
      <div class="fin-wk-header">
        <div>
          <div class="fin-ws-name">${esc(wk.name||'عامل بدون اسم')}</div>
          <div class="fin-ws-meta">
            <span class="badge ${typeCfg.badge||''}" style="font-size:10px;">${typeCfg.icon||''} ${esc(proj.projectCode)}</span>
            &nbsp; ${esc(client?.name||'—')}
            ${wk.job?`&nbsp;• ${esc(wk.job)}`:''}
            ${wk.phone?`&nbsp;• 📞 ${esc(wk.phone)}`:''}
          </div>
          <div class="fin-ws-meta" style="color:var(--accent);">
            ${fmt(wk.dailyWage||0,cur)}/يوم × ${wk.days||0} يوم = <strong>${fmt(total,cur)}</strong>
          </div>
        </div>
        <div style="display:flex;flex-direction:column;align-items:flex-end;gap:4px;">
          <span style="font-size:11px;color:var(--text3);">${wk.status||'—'}</span>
          ${wk.startDate?`<span style="font-size:10px;color:var(--text3);">بداية: ${wk.startDate}</span>`:''}
        </div>
      </div>
      <div class="fin-wk-kpis">
        <div class="fin-wk-kpi">
          <div class="fin-wk-kpi-lbl">التكلفة الإجمالية</div>
          <div class="fin-wk-kpi-val">${fmt(total,cur)}</div>
        </div>
        <div class="fin-wk-kpi">
          <div class="fin-wk-kpi-lbl" style="color:var(--green);">المدفوع (${paidPct}%)</div>
          <div class="fin-wk-kpi-val" style="color:var(--green);">${fmt(paid,cur)}</div>
        </div>
        <div class="fin-wk-kpi">
          <div class="fin-wk-kpi-lbl" style="color:${rem>0?'var(--red)':'var(--text3)'};">المستحق</div>
          <div class="fin-wk-kpi-val" style="color:${rem>0?'var(--red)':'var(--green)'};">${rem>0?fmt(rem,cur):'مسدد ✓'}</div>
        </div>
      </div>
      ${wk.payments.length?`<div class="fin-pay-ledger">
        <div class="fin-pay-ledger-title"><i class="ti ti-list-numbers"></i>سجل الدفعات (${wk.payments.length})</div>
        ${payRows}
      </div>`:''}
      ${rem>0 ? buildPayForm(wk.id,'wk',cur) : ''}
      <div class="fin-wk-footer">
        <div style="font-size:11px;color:var(--text3);">${wk.payments.length} دفعة مسجّلة</div>
        ${rem>0
          ? `<button class="fin-add-pay-btn" onclick="finOpenPay(${proj.id},'${wk.id}','wk')">
               <i class="ti ti-plus"></i> إضافة دفعة
             </button>`
          : `<span style="font-size:12px;color:var(--green);font-weight:700;">✅ تم السداد</span>`}
      </div>
    </div>`;
  }).join('');

  grid.innerHTML = summaryHtml + `<div class="cards-grid">${cardsHtml}</div>`;
}

// ── Main Finance Render (dispatches by FIN_TAB) ──
function renderFinance() {
  if(CU.role!=='manager') return;

  // Show/hide grids based on active tab
  if (typeof FIN_TAB !== 'undefined') {
    document.getElementById('finance-grid') ?.style.setProperty('display', FIN_TAB==='clients'?'':'none');
    document.getElementById('fin-ws-grid')  ?.style.setProperty('display', FIN_TAB==='ws'?'':'none');
    document.getElementById('fin-wk-grid')  ?.style.setProperty('display', FIN_TAB==='wk'?'':'none');
    if (FIN_TAB === 'ws') { renderFinanceWorkshops(); }
    if (FIN_TAB === 'wk') { renderFinanceWorkers(); }
    if (FIN_TAB !== 'clients') { /* update global KPIs but skip client grid */ }
  }

  const q  = (document.getElementById('fin2-search')?.value||'').toLowerCase();
  const fs = document.getElementById('fin2-filter-status')?.value||'';

  let gContract=0, gPaid=0, gExp=0;
  STATE.clients.forEach(c=>{
    const t = calcClientTotals(c.id);
    gContract += t.contractAmt; gPaid += t.paid; gExp += t.expenses;
  });
  const gRem = gContract - gPaid;
  const gNet = gPaid - gExp;
  document.getElementById('fin2-global-kpis').innerHTML = `
    <div class="fin2-kpi"><div class="fin2-kpi-lbl">قيمة العقود الكلية</div><div class="fin2-kpi-val">${fmt(gContract,'USD')}</div><div class="fin2-kpi-sub">${STATE.clients.length} عميل • ${STATE.projects.length} مشروع • $ تقريبي</div></div>
    <div class="fin2-kpi pos"><div class="fin2-kpi-lbl">إجمالي المحصّل</div><div class="fin2-kpi-val">${fmt(gPaid,'USD')}</div><div class="fin2-kpi-sub">${gContract?Math.round(gPaid/gContract*100):0}% من العقود</div></div>
    <div class="fin2-kpi warn"><div class="fin2-kpi-lbl">إجمالي المصروفات</div><div class="fin2-kpi-val">${fmt(gExp,'USD')}</div></div>
    <div class="fin2-kpi neg"><div class="fin2-kpi-lbl">المتبقي على العملاء</div><div class="fin2-kpi-val">${fmt(gRem,'USD')}</div></div>
    <div class="fin2-kpi ${gNet>=0?'pos':'neg'}"><div class="fin2-kpi-lbl">صافي الربح</div><div class="fin2-kpi-val">${fmt(gNet,'USD')}</div></div>`;

  let clients = STATE.clients;
  if(q) clients = clients.filter(c => c.name.toLowerCase().includes(q) || String(c.clientCode).toLowerCase().includes(q)
    || STATE.projects.some(p=>p.clientId===c.id&&(p.projectCode||'').toLowerCase().includes(q)));

  const grid = document.getElementById('finance-grid');
  if(!grid) return;
  if(!clients.length) { grid.innerHTML='<div class="empty" style="grid-column:1/-1;"><i class="ti ti-cash"></i><p>لا يوجد عملاء</p></div>'; return; }

  const cards = clients.map(c=>{
    const t = calcClientTotals(c.id);
    const projs = STATE.projects.filter(p=>p.clientId===c.id);
    if(fs==='has_debt' && t.remaining<=0) return '';
    if(fs==='paid' && t.remaining>0) return '';
    if(fs==='has_expenses' && t.expenses<=0) return '';
    const paidPct = t.contractAmt ? Math.round(t.paid/t.contractAmt*100) : 0;
    const projRows = projs.map(p=>{
      const pt = calcProjTotals(p);
      const statusCfg = STATUS[p.status]||{ar:p.status,badge:''};
      return `<div class="fin2-cc-proj-row" onclick="openProjFin(${p.id})">
        <div class="fin2-cc-proj-info">
          <span class="fin2-cc-proj-code">${esc(p.projectCode)}</span>
          <span class="fin2-cc-proj-desc" title="${esc(p.description)}">${esc(p.description||'—')}</span>
          <span class="badge ${statusCfg.badge}" style="font-size:10px;">${statusCfg.ar}</span>
        </div>
        <div class="fin2-cc-proj-amounts">
          <span style="color:var(--text3);font-size:10px;">عقد: ${fmt(pt.contractAmt, pt.cur||'USD')}</span>
          <span class="fin2-cc-paid">↓${fmt(pt.paid, pt.cur||'USD')}</span>
          ${pt.remaining>0?`<span class="fin2-cc-rem">↑${fmt(pt.remaining, pt.cur||'USD')}</span>`:'<span style="color:var(--green);font-size:11px;">✓ مسدد</span>'}
          <i class="ti ti-chevron-left" style="font-size:12px;color:var(--text3);"></i>
        </div>
      </div>`;
    }).join('');

    return `<div class="fin2-client-card">
      <div class="fin2-cc-header">
        <div>
          <div class="fin2-cc-name">${esc(c.name)}</div>
          <div class="fin2-cc-code">${esc(c.clientCode)} • ${t.projCount} مشروع</div>
        </div>
        <button class="tbtn" onclick="openClientFin(${c.id})" style="font-size:12px;padding:6px 12px;">
          <i class="ti ti-chart-bar"></i> ملخص مالي
        </button>
      </div>
      <div class="fin2-cc-kpis">
        <div class="fin2-cc-kpi"><div class="fin2-cc-kpi-lbl">قيمة العقود</div><div class="fin2-cc-kpi-val">${fmt(t.contractAmt, t.cur||'USD')}</div></div>
        <div class="fin2-cc-kpi"><div class="fin2-cc-kpi-lbl" style="color:var(--green);">المحصّل (${paidPct}%)</div><div class="fin2-cc-kpi-val" style="color:var(--green);">${fmt(t.paid, t.cur||'USD')}</div></div>
        <div class="fin2-cc-kpi"><div class="fin2-cc-kpi-lbl" style="color:${t.remaining>0?'var(--red)':'var(--text3)'};">المتبقي</div><div class="fin2-cc-kpi-val" style="color:${t.remaining>0?'var(--red)':'var(--green)'};">${t.remaining>0?fmt(t.remaining, t.cur||'USD'):'مسدد ✓'}</div></div>
      </div>
      ${projs.length?`<div class="fin2-cc-projects">${projRows}</div>`:'<div style="padding:12px 18px;font-size:12px;color:var(--text3);">لا توجد مشاريع</div>'}
      <div class="fin2-cc-footer">
        <button class="pfin-btn pfin-btn-income" onclick="openAddPaymentForClient(${c.id})" style="font-size:11px;padding:5px 10px;"><i class="ti ti-plus"></i> دفعة</button>
        <button class="pfin-btn pfin-btn-expense" onclick="openAddExpenseForClient(${c.id})" style="font-size:11px;padding:5px 10px;"><i class="ti ti-minus"></i> مصروف</button>
        <button class="pfin-btn pfin-btn-print" onclick="printClientStatement2(${c.id})" style="font-size:11px;padding:5px 10px;"><i class="ti ti-printer"></i> طباعة</button>
      </div>
    </div>`;
  }).filter(Boolean).join('');
  grid.innerHTML = cards || '<div class="empty" style="grid-column:1/-1;"><i class="ti ti-cash"></i><p>لا توجد نتائج مطابقة</p></div>';
}

function openProjFin(projectId) {
  PFIN_PROJECT_ID = projectId;
  PFIN_TAB = 'all';
  const p = STATE.projects.find(x=>x.id===projectId);
  if(!p) return;
  const c = STATE.clients.find(x=>x.id===p.clientId);
  const t = TYPES[p.taskTypeKey]||{};
  document.getElementById('pfin-title').textContent = p.projectCode + ' — ' + (t.ar||'');
  document.getElementById('pfin-sub').textContent = (c?.name||'—') + ' | ' + (p.description||'').slice(0,40);
  const projCur = getProjFin(p).currency || p.currency || 'USD';
  document.getElementById('pfin-currency').value = projCur;
  const cdisplay = document.getElementById('pfin-currency-display');
  if(cdisplay) cdisplay.textContent = (CURRENCY_SYMBOL[projCur]||projCur) + ' ' + projCur;
  renderProjKpis();
  renderProjLedger();
  switchPfinTab('all');
  document.getElementById('pfin-overlay').classList.add('open');
}
function closeProjFin() { document.getElementById('pfin-overlay').classList.remove('open'); }

function renderProjKpis() {
  const p = STATE.projects.find(x=>x.id===PFIN_PROJECT_ID);
  if(!p) return;
  const t = calcProjTotals(p);
  const cur = t.cur;
  const pct = t.contractAmt ? Math.round(t.paid/t.contractAmt*100) : 0;
  document.getElementById('pfin-kpis').innerHTML = `
    <div class="pfin-kpi kpi-blue"><div class="pfin-kpi-lbl">قيمة العقد</div><div class="pfin-kpi-val kpi-blue-val">${fmt(t.contractAmt,cur)}</div></div>
    <div class="pfin-kpi kpi-green"><div class="pfin-kpi-lbl">محصّل (${pct}%)</div><div class="pfin-kpi-val kpi-green-val">${fmt(t.paid,cur)}</div></div>
    <div class="pfin-kpi kpi-amber"><div class="pfin-kpi-lbl">إجمالي المصروفات</div><div class="pfin-kpi-val kpi-amber-val">${fmt(t.expenses,cur)}</div></div>
    <div class="pfin-kpi ${t.remaining>0?'kpi-red':'kpi-green'}"><div class="pfin-kpi-lbl">المتبقي على العميل</div><div class="pfin-kpi-val ${t.remaining>0?'kpi-red-val':'kpi-green-val'}">${t.remaining>0?fmt(t.remaining,cur):'مسدد ✓'}</div></div>
    <div class="pfin-kpi ${t.netProfit>=0?'kpi-acc':'kpi-red'}"><div class="pfin-kpi-lbl">صافي الربح</div><div class="pfin-kpi-val ${t.netProfit>=0?'kpi-acc-val':'kpi-red-val'}">${fmt(t.netProfit,cur)}</div></div>`;

  // Workforce cards for exec/super projects
  const wfEl = document.getElementById('pfin-wf-cards');
  if (!wfEl) return;
  if (!isExecType(p) || !p.workforce) { wfEl.style.display = 'none'; return; }
  const wft = calcWorkforceTotals(p);
  wfEl.style.display = '';
  wfEl.innerHTML = `<div class="wf-cards-strip">
    <!-- Workshops card -->
    <div class="wf-card">
      <div class="wf-card-title">🏭 الورشات والمقاولون</div>
      <div class="wf-card-row"><span class="wf-card-lbl">قيمة العقود</span><span class="wf-card-val">${fmt(wft.wsContract,cur)}</span></div>
      <div class="wf-card-row"><span class="wf-card-lbl">المدفوع</span><span class="wf-card-val green">${fmt(wft.wsPaid,cur)}</span></div>
      <div class="wf-card-row"><span class="wf-card-lbl">المتبقي</span><span class="wf-card-val ${wft.wsRem>0?'red':'green'}">${wft.wsRem>0?fmt(wft.wsRem,cur):'✓ مسدد'}</span></div>
    </div>
    <!-- Workers card -->
    <div class="wf-card">
      <div class="wf-card-title">👷 العمال</div>
      <div class="wf-card-row"><span class="wf-card-lbl">إجمالي التكلفة</span><span class="wf-card-val">${fmt(wft.wkCost,cur)}</span></div>
      <div class="wf-card-row"><span class="wf-card-lbl">المدفوع</span><span class="wf-card-val green">${fmt(wft.wkPaidAmt,cur)}</span></div>
      <div class="wf-card-row"><span class="wf-card-lbl">المستحق</span><span class="wf-card-val ${wft.wkRem>0?'amber':'green'}">${wft.wkRem>0?fmt(wft.wkRem,cur):'✓ مسدد'}</span></div>
    </div>
    <!-- Obligations card -->
    <div class="wf-card">
      <div class="wf-card-title">📋 إجمالي الالتزامات</div>
      <div class="wf-card-row"><span class="wf-card-lbl">ورشات + عمال</span><span class="wf-card-val">${fmt(wft.total,cur)}</span></div>
      <div class="wf-card-row"><span class="wf-card-lbl">إجمالي المدفوع</span><span class="wf-card-val green">${fmt(wft.totalPaid,cur)}</span></div>
      <div class="wf-card-row"><span class="wf-card-lbl">إجمالي المتبقي</span><span class="wf-card-val ${wft.totalRem>0?'red':'green'}">${wft.totalRem>0?fmt(wft.totalRem,cur):'✓ مسدد'}</span></div>
    </div>
  </div>`;
}

function switchPfinTab(tab) {
  PFIN_TAB = tab;
  ['all','income','expense'].forEach(t=>{
    document.getElementById('pfin-tab-'+t)?.classList.toggle('on', t===tab);
  });
  renderProjLedger();
}

function renderProjLedger() {
  const p = STATE.projects.find(x=>x.id===PFIN_PROJECT_ID);
  if(!p) return;
  const fin = getProjFin(p);
  const cur = fin.currency || p.currency || 'USD';
  let rows = [];
  if(PFIN_TAB!=='expense') {
    fin.payments.forEach(pm=>{
      rows.push({ type:'income', id:pm.id, date:pm.date||'', label:pm.label||'دفعة', amount:pm.amount, currency:pm.currency||fin.currency||'USD', notes:pm.notes||'', receipt:pm.receiptDataUrl||null, cat:null });
    });
  }
  if(PFIN_TAB!=='income') {
    fin.expenses.forEach(ex=>{
      rows.push({ type:'expense', id:ex.id, date:ex.date||'', label:ex.label||'مصروف', amount:ex.amount, currency:ex.currency||fin.currency||'USD', notes:ex.notes||'', receipt:ex.receiptDataUrl||null, cat:ex.category||'other' });
    });
  }
  rows.sort((a,b)=>(a.date||'').localeCompare(b.date||'') || a.id-b.id);
  const el = document.getElementById('pfin-ledger');
  if(!rows.length) {
    el.innerHTML = `<div class="empty" style="padding:40px;"><i class="ti ti-receipt-off"></i><p>لا توجد حركات مالية بعد</p></div>`;
    return;
  }
  const toDisp = (amt, srcCur) => {
    const sarAmt = amt || 0;  // no conversion
    const rate = EXCHANGE_RATES[cur]||1;
    return Math.round(sarAmt * rate);
  };
  let balance = 0;
  let html2 = `<table><thead><tr>
    <th>التاريخ</th><th>البيان</th><th>التصنيف</th><th style="color:var(--green);">وارد</th><th style="color:var(--red);">صادر</th><th>الرصيد</th><th></th>
  </tr></thead><tbody>`;
  rows.forEach(r=>{
    const disp = r.amount || 0;
    if(r.type==='income') balance += disp;
    else balance -= disp;
    const catCfg = r.cat ? (EXP_CATS[r.cat]||{ar:r.cat,icon:'📦'}) : null;
    const receiptHtml = r.receipt
      ? `<img src="${r.receipt}" class="pfin-receipt-thumb" onclick="showLightbox('${r.receipt}')" title="عرض الإيصال">`
      : '<span style="color:var(--text3);font-size:11px;">—</span>';
    const balColor = balance>=0?'var(--green)':'var(--red)';
    html2 += `<tr class="pfin-row-${r.type}">
      <td style="color:var(--text3);font-size:11px;white-space:nowrap;">${r.date||'—'}</td>
      <td>
        <div style="font-size:12.5px;font-weight:600;">${srcBadge}${esc(r.label)}</div>
        ${r.notes?`<div style="font-size:11px;color:var(--text3);">${esc(r.notes)}</div>`:''}
      </td>
      <td>${catCfg?`<span class="pfin-cat-badge">${catCfg.icon} ${catCfg.ar}</span>`:'<span style="color:var(--green);font-size:11px;">💰 دفعة عميل</span>'}</td>
      <td class="pfin-amount-income">${r.type==='income'?fmt(disp,cur):'—'}</td>
      <td class="pfin-amount-expense">${r.type==='expense'?fmt(disp,cur):'—'}</td>
      <td class="pfin-balance" style="color:${balColor};">${fmt(balance,cur)}</td>
      <td style="display:flex;gap:6px;align-items:center;">
        ${receiptHtml}
        <button class="icon-btn del" onclick="deleteTx(${r.id},'${r.type}')" title="حذف"><i class="ti ti-trash" style="font-size:13px;"></i> حذف</button>
      </td>
    </tr>`;
  });
  html2 += '</tbody></table>';
  el.innerHTML = html2;
}

function openAddPayment(projectId) {
  PFIN_PROJECT_ID = projectId || PFIN_PROJECT_ID;
  const p = STATE.projects.find(x=>x.id===PFIN_PROJECT_ID);
  if(!p) return;
  const fin = getProjFin(p);
  document.getElementById('add-pay-sub').textContent = p.projectCode + ' — ' + (STATE.clients.find(c=>c.id===p.clientId)?.name||'');
  document.getElementById('pay-amount').value='';
  const projCurr = fin.currency || p.currency || 'USD';
  document.getElementById('pay-currency').value = projCurr;
  // Lock currency to project currency — hide selector
  const payCurSel = document.getElementById('pay-currency');
  if(payCurSel) payCurSel.style.display='none';
  const payCurLbl = document.getElementById('pay-currency-label');
  if(payCurLbl) payCurLbl.textContent = CURRENCY_SYMBOL[projCurr]||projCurr;
  document.getElementById('pay-date').value = new Date().toISOString().split('T')[0];
  document.getElementById('pay-label').value = 'دفعة ' + (fin.payments.length+1);
  document.getElementById('pay-notes').value='';
  document.getElementById('pay-receipt-preview').style.display='none';
  document.getElementById('pay-receipt-preview').innerHTML='';
  PAY_RECEIPT_DATA = null;
  updatePayRemaining();
  document.getElementById('add-pay-overlay').classList.add('open');
}
function openAddPaymentForClient(clientId) {
  const projs = STATE.projects.filter(p=>p.clientId===clientId);
  if(projs.length===1) { openAddPayment(projs[0].id); return; }
  openClientFin(clientId);
}

function updatePayRemaining() {
  const amount = parseFloat(document.getElementById('pay-amount')?.value)||0;
  const p = STATE.projects.find(x=>x.id===PFIN_PROJECT_ID);
  if(!p) return;
  const t   = calcProjTotals(p);
  const cur = t.cur;
  const newRem = t.remaining - amount;
  const hint = document.getElementById('pay-remaining-hint');
  if(hint) hint.innerHTML = `المتبقي قبل هذه الدفعة: <strong>${fmt(t.remaining,cur)}</strong> → بعدها: <strong style="color:${newRem<=0?'var(--green)':'var(--amber)'};">${fmt(newRem,cur)}</strong>`;
}

function closeAddPayment() {
  document.getElementById('add-pay-overlay').classList.remove('open');
  PAY_RECEIPT_DATA = null;
}

function onPayReceiptSelected() {
  const inp = document.getElementById('pay-receipt-inp');
  const file = inp.files[0]; if(!file) return;
  const reader = new FileReader();
  reader.onload = e => {
    PAY_RECEIPT_DATA = e.target.result;
    const prev = document.getElementById('pay-receipt-preview');
    prev.style.display='flex';
    prev.innerHTML = `<img src="${PAY_RECEIPT_DATA}" alt="إيصال"><div style="font-size:11px;color:var(--text2);">${esc(file.name)}<br><button onclick="PAY_RECEIPT_DATA=null;document.getElementById('pay-receipt-preview').style.display='none';" style="background:none;border:none;cursor:pointer;color:var(--red);font-size:12px;">حذف ×</button></div>`;
  };
  reader.readAsDataURL(file);
  inp.value='';
}

async function savePayment() {
  const amount = parseFloat(document.getElementById('pay-amount').value)||0;
  const cur    = document.getElementById('pay-currency').value||'USD';
  const date   = document.getElementById('pay-date').value;
  const label  = document.getElementById('pay-label').value.trim()||'دفعة';
  if(!amount) { toast('⚠ أدخل المبلغ'); return; }
  if(!date)   { toast('⚠ أدخل التاريخ'); return; }
  const p = STATE.projects.find(x=>x.id===PFIN_PROJECT_ID);
  if(!p) return;
  const fin = getProjFin(p);
  fin.payments.push({ id:Date.now(), source:'manual', label, amount: amount, currency:cur, date, notes:document.getElementById('pay-notes').value.trim(), receiptDataUrl:PAY_RECEIPT_DATA||null });
  p.fin2 = fin;
  p.updatedAt = Date.now();
  await dbPut('projects', p);
  closeAddPayment();
  if(document.getElementById('pfin-overlay').classList.contains('open')) { renderProjKpis(); renderProjLedger(); }
  renderFinance();
  toast('✓ تم تسجيل الدفعة — ' + fmt(amount,cur));
}

function openAddExpense(projectId) {
  PFIN_PROJECT_ID = projectId || PFIN_PROJECT_ID;
  const p = STATE.projects.find(x=>x.id===PFIN_PROJECT_ID);
  if(!p) return;
  const fin = getProjFin(p);
  document.getElementById('add-exp-sub').textContent = p.projectCode + ' — ' + (STATE.clients.find(c=>c.id===p.clientId)?.name||'');
  document.getElementById('exp-amount').value='';
  const projCurrE = fin.currency || p.currency || 'USD';
  document.getElementById('exp-currency').value = projCurrE;
  const expCurSel = document.getElementById('exp-currency');
  if(expCurSel) expCurSel.style.display='none';
  const expCurLbl = document.getElementById('exp-currency-label');
  if(expCurLbl) expCurLbl.textContent = CURRENCY_SYMBOL[projCurrE]||projCurrE;
  document.getElementById('exp-date').value=new Date().toISOString().split('T')[0];
  document.getElementById('exp-label').value='';
  document.getElementById('exp-notes').value='';
  document.getElementById('exp-category').value='';
  document.getElementById('exp-receipt-preview').style.display='none';
  document.getElementById('exp-receipt-preview').innerHTML='';
  EXP_RECEIPT_DATA = null;
  document.querySelectorAll('.exp-cat-btn').forEach(b=>b.classList.remove('sel'));
  document.getElementById('add-exp-overlay').classList.add('open');
}
function openAddExpenseForClient(clientId) {
  const projs = STATE.projects.filter(p=>p.clientId===clientId);
  if(projs.length===1) { openAddExpense(projs[0].id); return; }
  openClientFin(clientId);
}

function selExpCat(btn) {
  document.querySelectorAll('.exp-cat-btn').forEach(b=>b.classList.remove('sel'));
  btn.classList.add('sel');
  document.getElementById('exp-category').value = btn.dataset.cat;
  const lbl = document.getElementById('exp-label');
  if(!lbl.value) lbl.value = EXP_CATS[btn.dataset.cat]?.ar||'';
}

function closeAddExpense() {
  document.getElementById('add-exp-overlay').classList.remove('open');
  EXP_RECEIPT_DATA = null;
}

function onExpReceiptSelected() {
  const inp = document.getElementById('exp-receipt-inp');
  const file = inp.files[0]; if(!file) return;
  const reader = new FileReader();
  reader.onload = e => {
    EXP_RECEIPT_DATA = e.target.result;
    const prev = document.getElementById('exp-receipt-preview');
    prev.style.display='flex';
    prev.innerHTML = `<img src="${EXP_RECEIPT_DATA}" alt="فاتورة"><div style="font-size:11px;color:var(--text2);">${esc(file.name)}<br><button onclick="EXP_RECEIPT_DATA=null;document.getElementById('exp-receipt-preview').style.display='none';" style="background:none;border:none;cursor:pointer;color:var(--red);font-size:12px;">حذف ×</button></div>`;
  };
  reader.readAsDataURL(file);
  inp.value='';
}

async function saveExpense() {
  const amount = parseFloat(document.getElementById('exp-amount').value)||0;
  const cur    = document.getElementById('exp-currency').value||'USD';
  const date   = document.getElementById('exp-date').value;
  const label  = document.getElementById('exp-label').value.trim();
  const cat    = document.getElementById('exp-category').value;
  if(!amount) { toast('⚠ أدخل المبلغ'); return; }
  if(!date)   { toast('⚠ أدخل التاريخ'); return; }
  if(!label)  { toast('⚠ أدخل وصف المصروف'); return; }
  if(!cat)    { toast('⚠ اختر تصنيف المصروف'); return; }
  const p = STATE.projects.find(x=>x.id===PFIN_PROJECT_ID);
  if(!p) return;
  const fin = getProjFin(p);
  fin.expenses.push({ id:Date.now(), source:'manual', category:cat, label, amount: amount, currency:cur, date, notes:document.getElementById('exp-notes').value.trim(), receiptDataUrl:EXP_RECEIPT_DATA||null });
  p.fin2 = fin;
  p.updatedAt = Date.now();
  await dbPut('projects', p);
  closeAddExpense();
  if(document.getElementById('pfin-overlay').classList.contains('open')) { renderProjKpis(); renderProjLedger(); }
  renderFinance();
  toast('✓ تم تسجيل المصروف — ' + fmt(amount,cur));
}

async function deleteTx(id, type) {
  if(!confirm('حذف هذه الحركة المالية؟')) return;
  const p = STATE.projects.find(x=>x.id===PFIN_PROJECT_ID);
  if(!p) return;
  const fin = getProjFin(p);
  if(type==='income')  fin.payments = fin.payments.filter(x=>x.id!==id);
  if(type==='expense') fin.expenses = fin.expenses.filter(x=>x.id!==id);
  p.fin2 = fin;
  await dbPut('projects', p);
  renderProjKpis(); renderProjLedger(); renderFinance();
  toast('تم الحذف');
}

function openClientFin(clientId) {
  CFIN_CLIENT_ID = clientId;
  const c = STATE.clients.find(x=>x.id===clientId);
  if(!c) return;
  document.getElementById('cfin-title').textContent = c.name;
  document.getElementById('cfin-sub').textContent   = c.clientCode + ' • ملخص مالي كامل';
  const projs = STATE.projects.filter(p=>p.clientId===clientId);
  const t = calcClientTotals(clientId);
  let body = `
    <div style="display:grid;grid-template-columns:repeat(3,1fr);gap:0;border-bottom:1px solid var(--border);">
      <div style="padding:14px 18px;border-left:1px solid var(--border);">
        <div style="font-size:10px;color:var(--text3);margin-bottom:3px;">قيمة العقود</div>
        <div style="font-size:18px;font-weight:700;">${fmt(t.contractAmt, t.cur||'USD')}</div>
      </div>
      <div style="padding:14px 18px;border-left:1px solid var(--border);">
        <div style="font-size:10px;color:var(--green);margin-bottom:3px;">المحصّل</div>
        <div style="font-size:18px;font-weight:700;color:var(--green);">${fmt(t.paid, t.cur||'USD')}</div>
      </div>
      <div style="padding:14px 18px;">
        <div style="font-size:10px;color:${t.remaining>0?'var(--red)':'var(--text3)'};margin-bottom:3px;">المتبقي</div>
        <div style="font-size:18px;font-weight:700;color:${t.remaining>0?'var(--red)':'var(--green)'};">${t.remaining>0?fmt(t.remaining, t.cur||'USD'):'مسدد ✓'}</div>
      </div>
    </div>
    <div style="display:grid;grid-template-columns:1fr 1fr;gap:0;border-bottom:1px solid var(--border);">
      <div style="padding:12px 18px;border-left:1px solid var(--border);">
        <div style="font-size:10px;color:var(--amber);margin-bottom:3px;">إجمالي المصروفات</div>
        <div style="font-size:16px;font-weight:700;color:var(--amber);">${fmt(t.expenses, t.cur||'USD')}</div>
      </div>
      <div style="padding:12px 18px;">
        <div style="font-size:10px;color:${t.netProfit>=0?'var(--accent)':'var(--red)'};margin-bottom:3px;">صافي الربح</div>
        <div style="font-size:16px;font-weight:700;color:${t.netProfit>=0?'var(--accent)':'var(--red)'};">${fmt(t.netProfit, t.cur||'USD')}</div>
      </div>
    </div>
    <div style="padding:14px 18px;">
      <div style="font-size:12px;font-weight:700;color:var(--text1);margin-bottom:10px;">تفاصيل المشاريع</div>
      <div style="overflow-x:auto;">
      <table class="cfin-proj-table">
        <thead><tr><th>المشروع</th><th>النوع</th><th>العقد</th><th>محصّل</th><th>مصروفات</th><th>متبقي</th><th>صافي</th><th></th></tr></thead>
        <tbody>${projs.map(p=>{
          const pt=calcProjTotals(p);
          const tCfg=TYPES[p.taskTypeKey]||{};
          return `<tr>
            <td><strong style="font-family:monospace;font-size:11px;">${esc(p.projectCode)}</strong></td>
            <td><span class="badge ${tCfg.badge||''}" style="font-size:10px;">${tCfg.icon||''} ${tCfg.ar||''}</span></td>
            <td>${fmt(pt.contractAmt, pt.cur||'USD')}</td>
            <td style="color:var(--green);">${fmt(pt.paid, pt.cur||'USD')}</td>
            <td style="color:var(--amber);">${fmt(pt.expenses, pt.cur||'USD')}</td>
            <td style="color:${pt.remaining>0?'var(--red)':'var(--green)'};">${pt.remaining>0?fmt(pt.remaining, pt.cur||'USD'):'✓'}</td>
            <td style="color:${pt.netProfit>=0?'var(--accent)':'var(--red)'};">${fmt(pt.netProfit, pt.cur||'USD')}</td>
            <td><button class="icon-btn edit" onclick="closeCFin();openProjFin(${p.id});" title="فتح المالية" style="display:flex;align-items:center;gap:4px;padding:5px 10px;border-radius:6px;"><i class="ti ti-external-link"></i> المالية</button></td>
          </tr>`;
        }).join('')}</tbody>
      </table>
      </div>
    </div>`;
  document.getElementById('cfin-body').innerHTML = body;
  document.getElementById('cfin-overlay').classList.add('open');
}
function closeCFin() { document.getElementById('cfin-overlay').classList.remove('open'); }

function printProjStatement() {
  const p = STATE.projects.find(x=>x.id===PFIN_PROJECT_ID);
  if(!p) return;
  const c   = STATE.clients.find(x=>x.id===p.clientId);
  const fin = getProjFin(p);
  const cur = fin.currency || p.currency || 'USD';
  const t   = calcProjTotals(p);

  let rows = [];
  fin.payments.forEach(pm=>rows.push({type:'income', ...pm}));
  fin.expenses.forEach(ex=>rows.push({type:'expense', ...ex}));
  rows.sort((a,b)=>(a.date||'').localeCompare(b.date||'')||a.id-b.id);
  let bal=0, rowsHtml='';
  rows.forEach(r=>{
    const disp = r.amount||0;
    if(r.type==='income') bal+=disp; else bal-=disp;
    const cat = r.category?(EXP_CATS[r.category]||{ar:r.category,icon:'📦'}):{ar:'دفعة عميل',icon:'💰'};
    rowsHtml+=`<tr style="border-bottom:1px solid #eee;">
      <td style="padding:8px 10px;color:#666;font-size:11px;">${r.date||'—'}</td>
      <td style="padding:8px 10px;font-size:11px;">${cat.icon} ${cat.ar}</td>
      <td style="padding:8px 10px;">${r.type==='income'?'<span style="color:#1D9E75;font-weight:700;">'+fmt(disp,cur)+'</span>':'—'}</td>
      <td style="padding:8px 10px;">${r.type==='expense'?'<span style="color:#E24B4A;font-weight:700;">'+fmt(disp,cur)+'</span>':'—'}</td>
      <td style="padding:8px 10px;font-weight:700;color:${bal>=0?'#1D9E75':'#E24B4A'};">${fmt(bal,cur)}</td>
      <td style="padding:8px 10px;font-size:11px;color:#666;">${r.label||''}</td>
    </tr>`;
  });
  const w = window.open('','_blank','width=860,height:1100');
  w.document.write(`<!DOCTYPE html><html dir="rtl" lang="ar"><head><meta charset="UTF-8">
    <title>كشف حساب ${p.projectCode}</title>
    <style>body{font-family:'Segoe UI',Tahoma,Arial,sans-serif;padding:30px;color:#1C1C1A;direction:rtl;}h1{font-size:20px;margin:0 0 4px;}h2{font-size:13px;color:#666;font-weight:400;margin:0 0 20px;}.kpis{display:grid;grid-template-columns:repeat(5,1fr);gap:10px;margin-bottom:20px;}.kpi{background:#f5f5f5;border-radius:8px;padding:12px;text-align:center;}.kpi-lbl{font-size:10px;color:#999;margin-bottom:4px;}.kpi-val{font-size:15px;font-weight:700;}table{width:100%;border-collapse:collapse;}th{background:#f0f0f0;padding:8px 10px;font-size:11px;text-align:right;border-bottom:2px solid #534AB7;}@media print{body{padding:15px;}}</style>
  </head><body>
    <h1>كشف حساب المشروع: ${p.projectCode}</h1>
    <h2>${c?.name||''} | ${p.description||''} | ${new Date().toLocaleDateString('ar-SA')}</h2>
    <div class="kpis">
      <div class="kpi"><div class="kpi-lbl">قيمة العقد</div><div class="kpi-val">${fmt(t.contractAmt,cur)}</div></div>
      <div class="kpi"><div class="kpi-lbl">المحصّل</div><div class="kpi-val" style="color:#1D9E75;">${fmt(t.paid,cur)}</div></div>
      <div class="kpi"><div class="kpi-lbl">المصروفات</div><div class="kpi-val" style="color:#EF9F27;">${fmt(t.expenses,cur)}</div></div>
      <div class="kpi"><div class="kpi-lbl">المتبقي</div><div class="kpi-val" style="color:#E24B4A;">${fmt(t.remaining,cur)}</div></div>
      <div class="kpi"><div class="kpi-lbl">صافي الربح</div><div class="kpi-val" style="color:#534AB7;">${fmt(t.netProfit,cur)}</div></div>
    </div>
    <table><thead><tr><th>التاريخ</th><th>التصنيف</th><th>وارد</th><th>صادر</th><th>الرصيد</th><th>البيان</th></tr></thead><tbody>${rowsHtml}</tbody></table>
    <div style="margin-top:30px;font-size:11px;color:#999;border-top:1px solid #eee;padding-top:10px;">طُبع من ProjexID — ${new Date().toLocaleString('ar-SA')}</div>
  
<!-- ══ WORKFORCE PAYMENT MODAL ═══════════════════════════════════ -->
<div class="overlay" id="wf-pay-overlay" style="z-index:950;"
  onclick="if(event.target===this)this.classList.remove('open')">
  <div class="modal" onclick="event.stopPropagation()" style="width:440px;">
    <div class="mhd">
      <div>
        <div class="mhd-t" id="wf-pay-title" style="color:var(--green);">💳 تسجيل دفعة</div>
        <div class="mhd-sub" id="wf-pay-info"></div>
      </div>
      <button class="icon-btn"
        onclick="document.getElementById('wf-pay-overlay').classList.remove('open')"><i class="ti ti-x"></i> إغلاق</button>
    </div>
    <div class="mbody">
      <!-- Payment type (workshops only) -->
      <div class="fg" id="wf-pay-type-row">
        <label>نوع الدفعة</label>
        <select class="fi" id="wf-pay-pay-type">
          <option value="advance">💵 دفعة مقدمة</option>
          <option value="milestone">🏁 دفعة مرحلية</option>
          <option value="final">✅ دفعة نهائية</option>
        </select>
      </div>
      <!-- Amount + date -->
      <div class="frow">
        <div class="fg">
          <label>المبلغ <span class="req">*</span></label>
          <input class="fi" type="number" id="wf-pay-amount" min="0" placeholder="0">
        </div>
        <div class="fg">
          <label>التاريخ <span class="req">*</span></label>
          <input class="fi" type="date" id="wf-pay-date">
        </div>
      </div>
      <!-- Method + reference -->
      <div class="frow">
        <div class="fg">
          <label>طريقة الدفع</label>
          <select class="fi" id="wf-pay-method">
            <option value="">اختر...</option>
            <option value="cash">نقداً</option>
            <option value="transfer">تحويل بنكي</option>
            <option value="cheque">شيك</option>
            <option value="other">أخرى</option>
          </select>
        </div>
        <div class="fg">
          <label>المرجع / رقم العملية</label>
          <input class="fi" id="wf-pay-ref" placeholder="اختياري">
        </div>
      </div>
      <div class="fg">
        <label>ملاحظات</label>
        <textarea class="fi" id="wf-pay-notes"
          placeholder="(اختياري)" style="min-height:55px;"></textarea>
      </div>
    </div>
    <div class="mft">
      <button class="btn-cancel"
        onclick="document.getElementById('wf-pay-overlay').classList.remove('open')">إلغاء</button>
      <button class="btn-save" style="background:var(--green);" onclick="fuWfPaySave()">
        <i class="ti ti-check" style="vertical-align:-2px;margin-left:4px;"></i> تأكيد الدفعة
      </button>
    </div>
  </div>
</div>


<!-- Task detail drawer -->
<div class="pf-drawer" id="pf-drawer" onclick="if(event.target===this||event.target.classList.contains('pf-drawer-overlay'))pfCloseTask();">
  <div class="pf-drawer-overlay"></div>
  <div class="pf-drawer-panel" id="pf-drawer-panel">
    <div class="pf-drawer-hdr">
      <div style="flex:1;">
        <div id="pf-dt-status-badge"></div>
        <div id="pf-dt-name" style="font-size:16px;font-weight:700;margin-top:4px;"></div>
        <div id="pf-dt-meta" style="font-size:11px;color:var(--text3);margin-top:3px;"></div>
      </div>
      <button onclick="pfCloseTask()" style="background:none;border:none;cursor:pointer;font-size:20px;color:var(--text3);padding:4px 8px;">✕ إغلاق</button>
    </div>
    <div class="pf-drawer-tabs" id="pf-drawer-tabs"></div>
    <div class="pf-drawer-body" id="pf-drawer-body"></div>
  </div>
</div>


<script>
// ── Startup: check session then show login or app ──
(async function startApp() {
  await initDB();
  // Load dynamic users first
  try {
    const uSaved = localStorage.getItem('pxid_users');
    DUSERS = uSaved ? JSON.parse(uSaved) : null;
  } catch(e) { DUSERS = null; }

  const restored = tryRestoreSession();
  if (restored) {
    // Valid session — go straight to app
    await loadAllData();
    document.getElementById('login-wrap').style.display = 'none';
    document.getElementById('app').style.display = 'flex';
    applyRoleUI();
    renderAll();
  } else {
    // No session — show login
    document.getElementById('login-wrap').style.display = 'flex';
    document.getElementById('app').style.display = 'none';
  }
})();
</script>
</body></html>`);
  w.document.close();
  setTimeout(()=>w.print(),500);
}

function printClientStatement2(clientId) {
  CFIN_CLIENT_ID = clientId||CFIN_CLIENT_ID;
  const c = STATE.clients.find(x=>x.id===CFIN_CLIENT_ID); if(!c) return;
  const t = calcClientTotals(CFIN_CLIENT_ID);
  const projs = STATE.projects.filter(p=>p.clientId===CFIN_CLIENT_ID);
  const projRows = projs.map(p=>{const pt=calcProjTotals(p);return `<tr style="border-bottom:1px solid #eee;"><td style="padding:8px 10px;font-family:monospace;">${p.projectCode}</td><td style="padding:8px 10px;">${p.description||'—'}</td><td style="padding:8px 10px;">${fmt(pt.contractAmt, pt.cur||'USD')}</td><td style="padding:8px 10px;color:#1D9E75;">${fmt(pt.paid, pt.cur||'USD')}</td><td style="padding:8px 10px;color:#EF9F27;">${fmt(pt.expenses, pt.cur||'USD')}</td><td style="padding:8px 10px;color:${pt.remaining>0?'#E24B4A':'#1D9E75'};">${pt.remaining>0?fmt(pt.remaining, pt.cur||'USD'):'✓ مسدد'}</td></tr>`; }).join('');
  const w=window.open('','_blank','width=860,height:1100');
  w.document.write(`<!DOCTYPE html><html dir="rtl" lang="ar"><head><meta charset="UTF-8"><title>كشف ${c.name}</title><style>body{font-family:'Segoe UI',Tahoma,Arial,sans-serif;padding:30px;color:#1C1C1A;direction:rtl;}table{width:100%;border-collapse:collapse;}th{background:#f0f0f0;padding:8px 10px;font-size:11px;text-align:right;}</style></head><body>
    <h1>ملخص الحساب: ${c.name}</h1><p>${c.clientCode} | ${new Date().toLocaleDateString('ar-SA')}</p>
    <div style="display:grid;grid-template-columns:repeat(5,1fr);gap:10px;margin:16px 0;">${[['قيمة العقود',t.contractAmt,'#1C1A3A'],['المحصّل',t.paid,'#1D9E75'],['المصروفات',t.expenses,'#EF9F27'],['المتبقي',t.remaining,'#E24B4A'],['صافي الربح',t.netProfit,'#534AB7']].map(([l,v,col])=>`<div style="background:#f5f5f5;border-radius:8px;padding:12px;text-align:center;"><div style="font-size:10px;color:#999;margin-bottom:4px;">${l}</div><div style="font-size:14px;font-weight:700;color:${col};">${fmt(v,'USD')}</div></div>`).join('')}</div>
    <table><thead><tr><th>المشروع</th><th>الوصف</th><th>العقد</th><th>محصّل</th><th>مصروفات</th><th>متبقي</th></tr></thead><tbody>${projRows}</tbody></table>
  
<script>
// ── Startup: check session then show login or app ──
(async function startApp() {
  await initDB();
  // Load dynamic users first
  try {
    const uSaved = localStorage.getItem('pxid_users');
    DUSERS = uSaved ? JSON.parse(uSaved) : null;
  } catch(e) { DUSERS = null; }

  const restored = tryRestoreSession();
  if (restored) {
    // Valid session — go straight to app
    await loadAllData();
    document.getElementById('login-wrap').style.display = 'none';
    document.getElementById('app').style.display = 'flex';
    applyRoleUI();
    renderAll();
  } else {
    // No session — show login
    document.getElementById('login-wrap').style.display = 'flex';
    document.getElementById('app').style.display = 'none';
  }
})();
</script>
</body></html>`);
  w.document.close(); setTimeout(()=>w.print(),500);
}

function printClientStatement() { printClientStatement2(CFIN_CLIENT_ID); }

function exportProjCsv() {
  const p = STATE.projects.find(x=>x.id===PFIN_PROJECT_ID); if(!p) return;
  const fin = getProjFin(p);
  const cur = fin.currency || p.currency || 'USD';
  let rows = [];
  fin.payments.forEach(pm=>rows.push({type:'دفعة عميل',date:pm.date,label:pm.label,amount:pm.amount||0,currency:cur,cat:'',notes:pm.notes}));
  fin.expenses.forEach(ex=>rows.push({type:'مصروف',date:ex.date,label:ex.label,amount:-(ex.amount||0),currency:cur,cat:(EXP_CATS[ex.category]||{ar:ex.category}).ar,notes:ex.notes}));
  rows.sort((a,b)=>(a.date||'').localeCompare(b.date||''));
  const csv = 'التاريخ,النوع,البيان,التصنيف,المبلغ,العملة,الملاحظات\n' + rows.map(r=>[r.date,r.type,r.label,r.cat,r.amount,r.currency,r.notes].map(v=>`"${String(v||'').replace(/"/g,"'")}"`).join(',')).join('\n');
  const blob = new Blob(['﻿'+csv],{type:'text/csv;charset=utf-8'});
  const a=document.createElement('a'); a.href=URL.createObjectURL(blob); a.download=p.projectCode+'_finance.csv'; a.click();
  toast('تم تصدير الملف CSV');
}

function exportGlobalFinance() {
  let rows=[];
  STATE.projects.forEach(p=>{
    const fin=getProjFin(p);
    const c=STATE.clients.find(x=>x.id===p.clientId);
    fin.payments.forEach(pm=>rows.push({proj:p.projectCode,client:c?.name||'',type:'دفعة عميل',date:pm.date,label:pm.label,amount:pm.amount||0,currency:fin.currency||'USD',cat:'',notes:pm.notes}));
    fin.expenses.forEach(ex=>rows.push({proj:p.projectCode,client:c?.name||'',type:'مصروف',date:ex.date,label:ex.label,amount:-toSAR(ex.amount,ex.currency),cat:(EXP_CATS[ex.category]||{ar:ex.category}).ar,notes:ex.notes}));
  });
  rows.sort((a,b)=>(a.date||'').localeCompare(b.date||''));
  const csv='المشروع,العميل,التاريخ,النوع,البيان,التصنيف,المبلغ\n'
    +rows.map(r=>[r.proj,r.client,r.date,r.type,r.label,r.cat,r.amount].map(v=>`"${String(v||'').replace(/"/g,"'")}"`).join(',')).join('\n');
  const blob=new Blob(['﻿'+csv],{type:'text/csv;charset=utf-8'});
  const a=document.createElement('a'); a.href=URL.createObjectURL(blob); a.download='ProjexID_finance_'+new Date().toISOString().split('T')[0]+'.csv'; a.click();
  toast('تم تصدير الملف الشامل');
}

function printGlobalStatement() { window.print(); }

function showLightbox(src) {
  document.getElementById('lightbox-img').src=src;
  document.getElementById('lightbox-overlay').classList.add('open');
}
function closeLightbox() { document.getElementById('lightbox-overlay').classList.remove('open'); }

function openFinModal(clientId) { openClientFin(clientId); }
function closeFinModal() {}
function addFinPayment() {}
function removeFinPayment(i) {}
async function saveFinData() {}

// ══════════════════════════════════════════════════════════════════
// REPORTS
// ══════════════════════════════════════════════════════════════════
let REP_FILES = []; // pending files for new report
let REP_DETAIL_ID = null; // currently viewed report id

const REP_TYPE_CFG = {
  daily:      { ar: 'يومي',              icon: '📅', cls: 'rep-type-daily' },
  weekly:     { ar: 'أسبوعي',            icon: '📊', cls: 'rep-type-weekly' },
  milestone:  { ar: 'مرحلي',             icon: '🏁', cls: 'rep-type-milestone' },
  final:      { ar: 'نهائي',             icon: '✅', cls: 'rep-type-final' },
  daily_site: { ar: 'سجل يومي للموقع',  icon: '🏗️', cls: 'rep-type-daily' }
};

const FILE_ICONS = {
  pdf:'ti-file-type-pdf', jpg:'ti-photo', jpeg:'ti-photo', png:'ti-photo',
  gif:'ti-photo', webp:'ti-photo', dwg:'ti-vector', dxf:'ti-vector',
  docx:'ti-file-word', doc:'ti-file-word', xlsx:'ti-file-spreadsheet',
  xls:'ti-file-spreadsheet', zip:'ti-file-zip', rar:'ti-file-zip',
  ifc:'ti-cube', mp4:'ti-video', mov:'ti-video'
};

function getFileIcon(name) {
  const ext = (name||'').split('.').pop().toLowerCase();
  return FILE_ICONS[ext] || 'ti-file';
}

function isImage(name) {
  return /\.(jpg|jpeg|png|gif|webp)$/i.test(name||'');
}

// ── Render hero banner ──
function renderRepBanner(list) {
  const banner = document.getElementById('rep-hero-banner');
  if(!banner) return;
  const total = list.length;
  const byType = {};
  list.forEach(r => { byType[r.reportType] = (byType[r.reportType]||0)+1; });
  banner.innerHTML = `
    <div class="rep-hero">
      <div>
        <div class="rep-hero-title"><i class="ti ti-report-analytics" style="vertical-align:-3px;margin-left:8px;"></i>سجل التقارير</div>
        <div class="rep-hero-sub">جميع التقارير المرفوعة من المهندسين</div>
      </div>
      <div class="rep-stat-pills">
        <div class="rep-stat-pill"><i class="ti ti-files"></i><span>الإجمالي</span><strong>${total}</strong></div>
        ${Object.entries(REP_TYPE_CFG).map(([k,v])=>byType[k]?`<div class="rep-stat-pill">${v.icon} <span>${v.ar}</span><strong>${byType[k]}</strong></div>`:'').join('')}
      </div>
    </div>`;
}

// ── Populate filter dropdowns ──
function populateRepFilters() {
  // Engineers
  const engSel = document.getElementById('rep-filter-eng');
  if(engSel && engSel.options.length <= 1) {
    STATE.engineers.forEach(e => {
      const o = document.createElement('option');
      o.value = e.id; o.textContent = e.name; engSel.appendChild(o);
    });
  }
  // Projects
  const projSel = document.getElementById('rep-filter-proj');
  if(projSel && projSel.options.length <= 1) {
    STATE.projects.forEach(p => {
      const o = document.createElement('option');
      o.value = p.id; o.textContent = p.projectCode + (p.description?' — '+p.description.slice(0,25):'');
      projSel.appendChild(o);
    });
  }
  // Workshops (collected from all exec projects)
  const wsSel = document.getElementById('rep-filter-ws');
  if(wsSel && wsSel.options.length <= 1) {
    const wsSet = new Set();
    STATE.projects.filter(p=>isExecType(p)).forEach(p=>{
      (p.workforce?.workshops||[]).forEach(s=>{ if(s.name||s.type) wsSet.add(s.name||s.type); });
    });
    wsSet.forEach(name => {
      const o = document.createElement('option');
      o.value = name; o.textContent = name; wsSel.appendChild(o);
    });
  }
}

// ── Render the full projects list shown above filtered reports ──
function renderRepAllProjects() {
  const box = document.getElementById('rep-all-projects');
  if(!box) return;
  const projects = [...STATE.projects].sort((a,b)=>b.createdAt-a.createdAt);
  if(!projects.length) { box.innerHTML=''; return; }
  box.innerHTML = `
    <div style="background:var(--surface);border:1px solid var(--border);border-radius:var(--radius);padding:14px;">
      <div style="display:flex;align-items:center;gap:8px;margin-bottom:10px;font-weight:600;color:var(--text1);">
        <i class="ti ti-folders"></i>
        <span>جميع المشاريع (${projects.length})</span>
      </div>
      <div style="display:grid;grid-template-columns:repeat(auto-fill,minmax(220px,1fr));gap:8px;">
        ${projects.map(p=>{
          const c = STATE.clients.find(cl=>cl.id===p.clientId);
          const t = TYPES[p.taskTypeKey]?.ar || p.taskTypeArabic || '';
          return `<div style="background:var(--surface2);border:1px solid var(--border);border-radius:var(--radius-sm);padding:8px 10px;">
            <div style="font-size:12px;font-weight:600;color:var(--accent);">${p.projectCode||''}</div>
            <div style="font-size:12px;color:var(--text1);margin-top:2px;">${t}</div>
            <div style="font-size:11px;color:var(--text3);margin-top:2px;">${c?c.name:''}</div>
          </div>`;
        }).join('')}
      </div>
    </div>`;
}

// ── Main render ──
// ═══ REPORTS GROUPING ════════════════════════════════════════════
let REP_GROUP = 'none'; // 'none'|'project'|'client'|'engineer'

function setRepGroup(group) {
  REP_GROUP = group;
  ['none','project','client','engineer'].forEach(g => {
    document.getElementById('rg-'+g)?.classList.toggle('on', g===group);
  });
  // Hide/show simple filters when grouping is active
  const filterBar = document.getElementById('rep-filter-bar');
  if(filterBar) filterBar.style.display = group==='none' ? '' : 'none';
  const repBackBtn = document.getElementById('rep-back-btn');
  if(repBackBtn) repBackBtn.style.display = group!=='none' ? '' : 'none';
  renderReports();
}

// Click-to-filter: set a filter value and re-render in 'none' mode
function repFilterBy(type, value) {
  setRepGroup('none');
  if(type==='project') {
    const sel = document.getElementById('rep-filter-proj');
    if(sel) { sel.value = value; renderReports(); }
  } else if(type==='engineer') {
    const sel = document.getElementById('rep-filter-eng');
    if(sel) { sel.value = value; renderReports(); }
  }
}

// Toggle a group accordion
function repToggleGroup(id) {
  const hdr  = document.getElementById('rep-gh-'+id);
  const body = document.getElementById('rep-gb-'+id);
  if(!hdr||!body) return;
  const open = body.classList.toggle('open');
  hdr.classList.toggle('open', open);
  const ico = hdr.querySelector('.rep-group-chevron');
  if(ico) ico.style.transform = open ? 'rotate(180deg)' : '';
}
function repToggleSub(id) {
  const hdr  = document.getElementById('rep-sh-'+id);
  const body = document.getElementById('rep-sb-'+id);
  if(!hdr||!body) return;
  const open = body.classList.toggle('open');
  hdr.classList.toggle('open', open);
}
// Inline toggle for sub-headers without IDs
function repSubToggle(el) {
  el.classList.toggle('open');
  const body = el.nextElementSibling;
  if(body) body.classList.toggle('open');
}

// Build report cards for a list
function repCards(list) {
  if(!list.length) return '<div style="color:var(--text3);font-size:12px;padding:8px 0;">لا توجد تقارير</div>';
  return `<div class="rep-cards-row">${list.map(r=>{
    try {
      return r.reportType==='daily_site' ? renderDailyLogCard(r) : renderRepCard(r);
    } catch(e) { return ''; }
  }).join('')}</div>`;
}

// ── Group by PROJECT ──────────────────────────────────────────────
function renderRepGroupProject(list) {
  const grid = document.getElementById('reports-grid');
  if(!grid) return;
  grid.style.display = 'block';

  // Start from ALL projects (not just those with reports)
  let projects = [...STATE.projects].sort((a,b)=>(a.projectCode||'').localeCompare(b.projectCode||''));

  if(!projects.length) {
    grid.innerHTML = '<div class="empty" style="grid-column:1/-1;"><i class="ti ti-folder"></i><p>لا توجد مشاريع</p></div>';
    return;
  }

  grid.innerHTML = projects.map((p,i)=>{
    const c   = STATE.clients.find(cl=>cl.id===p.clientId);
    const t   = TYPES[p.taskTypeKey]||{};
    // Reports belonging to this project
    const projReports = list.filter(r=>r.projectId===p.id);
    const projBlock   = repProjBlock(p, projReports, true);

    return `<div class="rep-group-section">
      <div class="rep-group-header open" id="rep-gh-proj-${i}" onclick="repToggleGroup('proj-${i}')">
        <div class="rep-group-title">
          <div class="rep-group-icon" style="background:var(--accent-light);color:var(--accent);">
            ${t.icon||'📁'}
          </div>
          <div>
            <div class="rep-group-name" style="font-family:monospace;">${esc(p.projectCode)}</div>
            <div class="rep-group-meta">
              ${esc(c?.name||'—')}
              ${p.description?' — '+esc(p.description.slice(0,35)):''}
              &nbsp;•&nbsp; <span class="badge ${t.badge||''}" style="font-size:9px;">${t.ar||''}</span>
            </div>
          </div>
        </div>
        <div class="rep-group-right">
          <span class="rep-count-badge"><i class="ti ti-report"></i>${projReports.length} تقرير</span>
          <i class="ti ti-chevron-down rep-group-chevron" style="transform:rotate(180deg);"></i>
        </div>
      </div>
      <div class="rep-group-body open" id="rep-gb-proj-${i}">
        ${projBlock}
      </div>
    </div>`;
  }).join('');
}

// ── Group by CLIENT ───────────────────────────────────────────────
function renderRepGroupClient(list) {
  const grid = document.getElementById('reports-grid');
  if(!grid) return;
  grid.style.display = 'block';

  // Group projects by client
  const clientMap = {};
  STATE.projects.forEach(p=>{
    const c = STATE.clients.find(cl=>cl.id===p.clientId);
    const key = c ? String(c.id) : 'none';
    const cName = c?.name || 'عميل غير معروف';
    if(!clientMap[key]) clientMap[key] = { id:c?.id, name:cName, phone:c?.phone||'', projects:[] };
    clientMap[key].projects.push(p);
  });

  const clientList = Object.values(clientMap).sort((a,b)=>a.name.localeCompare(b.name));
  if(!clientList.length) {
    grid.innerHTML='<div class="empty" style="grid-column:1/-1;"><i class="ti ti-users"></i><p>لا يوجد عملاء</p></div>';
    return;
  }

  grid.innerHTML = clientList.map((cl,ci)=>{
    const totalReps = cl.projects.reduce((s,p)=>s+list.filter(r=>r.projectId===p.id).length,0);
    const subGroups = cl.projects.map((p,pi)=>{
      const projReports = list.filter(r=>r.projectId===p.id);
      return repProjBlock(p, projReports, true);
    }).join('');

    return `<div class="rep-group-section">
      <div class="rep-group-header open" id="rep-gh-cl-${ci}" onclick="repToggleGroup('cl-${ci}')">
        <div class="rep-group-title">
          <div class="rep-group-icon" style="background:var(--blue-light);color:var(--blue);">👤</div>
          <div>
            <div class="rep-group-name">${esc(cl.name)}</div>
            <div class="rep-group-meta">
              ${cl.projects.length} مشروع
              ${cl.phone?' • 📞 '+esc(cl.phone):''}
            </div>
          </div>
        </div>
        <div class="rep-group-right">
          <span class="rep-count-badge"><i class="ti ti-report"></i>${totalReps} تقرير</span>
          <i class="ti ti-chevron-down rep-group-chevron" style="transform:rotate(180deg);"></i>
        </div>
      </div>
      <div class="rep-group-body open" id="rep-gb-cl-${ci}">
        ${subGroups}
      </div>
    </div>`;
  }).join('');
}

// ── Group by ENGINEER ─────────────────────────────────────────────
function renderRepGroupEngineer(list) {
  const grid = document.getElementById('reports-grid');
  if(!grid) return;
  grid.style.display = 'block';

  // Group projects by assigned engineer
  const engMap = {};
  // Add "unassigned" slot
  engMap['none'] = { eng:null, name:'غير مسند', projects:[] };
  STATE.engineers.forEach(e=>{
    engMap[String(e.id)] = { eng:e, name:e.name, projects:[] };
  });
  STATE.projects.forEach(p=>{
    const key = p.engineerId ? String(p.engineerId) : 'none';
    if(engMap[key]) engMap[key].projects.push(p);
    else engMap['none'].projects.push(p);
  });

  // Sort: engineers with projects first
  const engList = Object.values(engMap)
    .filter(g=>g.projects.length>0)
    .sort((a,b)=>{
      if(!a.eng) return 1; if(!b.eng) return -1;
      return a.name.localeCompare(b.name);
    });

  if(!engList.length) {
    grid.innerHTML='<div class="empty" style="grid-column:1/-1;"><i class="ti ti-hard-hat"></i><p>لا يوجد مهندسون</p></div>';
    return;
  }

  grid.innerHTML = engList.map((group,ei)=>{
    const initials = group.name.split(' ').map(w=>w[0]).slice(0,2).join('');
    const totalReps = group.projects.reduce((s,p)=>s+list.filter(r=>r.projectId===p.id).length,0);
    const subGroups = group.projects.map((p,pi)=>{
      const projReports = list.filter(r=>r.projectId===p.id);
      return repProjBlock(p, projReports, true);
    }).join('');

    return `<div class="rep-group-section">
      <div class="rep-group-header open" id="rep-gh-en-${ei}" onclick="repToggleGroup('en-${ei}')">
        <div class="rep-group-title">
          <div class="rep-group-icon" style="background:var(--green-light);color:var(--green);
            font-size:13px;font-weight:700;">${esc(initials||'؟')}</div>
          <div>
            <div class="rep-group-name">${esc(group.name)}</div>
            <div class="rep-group-meta">
              ${group.eng?.specialty||''}
              ${group.eng?.phone?' • 📞 '+esc(group.eng.phone):''}
              &nbsp;•&nbsp; ${group.projects.length} مشروع
            </div>
          </div>
        </div>
        <div class="rep-group-right">
          <span class="rep-count-badge"><i class="ti ti-report"></i>${totalReps} تقرير</span>
          <i class="ti ti-chevron-down rep-group-chevron" style="transform:rotate(180deg);"></i>
        </div>
      </div>
      <div class="rep-group-body open" id="rep-gb-en-${ei}">
        ${subGroups}
      </div>
    </div>`;
  }).join('');
}

function renderReports() {
  populateRepFilters();

  const ft   = document.getElementById('rep-filter-type')?.value||'';
  const fe   = document.getElementById('rep-filter-eng')?.value||'';

  let list = [...STATE.reports];

  // Engineer scope
  if(CU.role==='engineer') {
    const eng = STATE.engineers.find(e=>e.name===CU.name||e.username===CU.username);
    if(eng) list = list.filter(r=>r.engineerId===eng.id);
  }

  // Filters
  const fp   = document.getElementById('rep-filter-proj')?.value||'';
  const fws  = document.getElementById('rep-filter-ws')?.value||'';
  const fFrom= document.getElementById('rep-filter-from')?.value||'';
  const fTo  = document.getElementById('rep-filter-to')?.value||'';
  const sort = document.getElementById('rep-sort')?.value||'newest';

  if(ft)    list = list.filter(r=>r.reportType===ft);
  if(fe)    list = list.filter(r=>String(r.engineerId)===fe);
  if(fp)    list = list.filter(r=>String(r.projectId)===fp);
  if(fws)   list = list.filter(r=>(r.workshop||'').includes(fws));
  if(fFrom) list = list.filter(r=>(r.date||'')>=fFrom);
  if(fTo)   list = list.filter(r=>(r.date||'')<=fTo);

  // Sort
  if(sort==='newest')   list.sort((a,b)=>b.createdAt-a.createdAt);
  if(sort==='oldest')   list.sort((a,b)=>a.createdAt-b.createdAt);
  if(sort==='project')  list.sort((a,b)=>(a.projectCode||'').localeCompare(b.projectCode||''));
  if(sort==='workshop') list.sort((a,b)=>(a.workshop||'').localeCompare(b.workshop||''));
  if(sort==='engineer') list.sort((a,b)=>(a.engineerName||'').localeCompare(b.engineerName||''));

  // ── Dispatch to group renderers ──────────────────────────────
  { const gGrid = document.getElementById('reports-grid');
    if(gGrid) gGrid.style.display = ''; }

  if(REP_GROUP === 'project')  { renderRepGroupProject(list);  return; }
  if(REP_GROUP === 'client')   { renderRepGroupClient(list);   return; }
  if(REP_GROUP === 'engineer') { renderRepGroupEngineer(list); return; }

  // Render the "all projects" list above the filtered reports (none-group only)
  renderRepAllProjects();

  // Banner (on full unfiltered list)
  renderRepBanner(STATE.reports.filter(r => {
    if(CU.role!=='engineer') return true;
    const eng = STATE.engineers.find(e=>e.name===CU.name||e.username===CU.username);
    return eng?r.engineerId===eng.id:true;
  }));

  const grid = document.getElementById('reports-grid');
  if(!grid) return;
  if(!list.length) {
    grid.innerHTML='<div class="empty" style="grid-column:1/-1;"><i class="ti ti-report"></i><p>لا توجد تقارير مطابقة</p></div>';
    return;
  }

  grid.innerHTML = list.map(r=>{
    // daily_site — use dedicated card renderer
    if(r.reportType==='daily_site') {
      try { return renderDailyLogCard(r); } catch(e) { console.error('renderDailyLogCard error',e,r); return ''; }
    }

    const proj = STATE.projects.find(pr=>pr.id===r.projectId);
    const eng  = STATE.engineers.find(en=>en.id===r.engineerId);
    const rt   = REP_TYPE_CFG[r.reportType] || { ar:r.reportType, icon:'📄', cls:'' };
    const prog = r.progressSnapshot;
    const files = r.attachments||[];
    const imgFiles = files.filter(f=>isImage(f.name));
    const hasFiles = files.length > 0;

    return `
    <div class="rep-card" onclick="openRepDetail('${r.id}')">
      <div class="rep-card-top">
        <div style="display:flex;flex-direction:column;gap:4px;">
          <span class="rep-num">${esc(r.reportNumber||'—')}</span>
          <span class="rep-type-badge ${rt.cls}">${rt.icon} ${rt.ar}</span>
        </div>
        <div style="text-align:left;">
          <div class="rep-date">${r.date||''}</div>
          ${hasFiles?`<div class="rep-files-tag" style="margin-top:4px;"><i class="ti ti-paperclip"></i>${files.length} مرفق</div>`:''}
        </div>
      </div>
      <div class="rep-proj-name">${esc(proj?.description?.slice(0,45)||'—')}</div>
      <div class="rep-proj-code">
        <i class="ti ti-hash" style="font-size:11px;color:var(--accent);"></i>
        ${esc(proj?.projectCode||'—')}
        <span style="color:var(--border2);">|</span>
        <i class="ti ti-${getFileIcon(proj?.taskTypeKey)}" style="font-size:11px;"></i>
        ${esc((REP_TYPES[proj?.taskTypeKey]||{}).ar||proj?.taskTypeKey||'—')}
      </div>
      ${prog!=null?`
      <div class="rep-prog-row">
        <div class="rep-prog-label"><span>لقطة الإنجاز</span><strong>${prog}%</strong></div>
        <div class="prog-bar" style="height:6px;"><div class="prog-fill" style="width:${prog}%;${prog===100?'background:var(--green);':''}"></div></div>
      </div>`:''}
      <div class="rep-content-preview">${esc(r.content||'')}</div>
      <div class="rep-footer">
        <div class="rep-eng-tag">
          <i class="ti ti-hard-hat"></i>
          ${esc(eng?.name||'—')}
        </div>
        <div style="display:flex;align-items:center;gap:6px;">
          ${imgFiles.length?`<img src="${imgFiles[0].dataUrl||''}" style="width:26px;height:26px;object-fit:cover;border-radius:4px;border:1px solid var(--border);" onerror="this.style.display='none'">`:''}
          <i class="ti ti-chevron-left" style="font-size:14px;color:var(--text3);"></i>
        </div>
      </div>
    </div>`;
  }).join('');
}

// ── Open Report Modal ──
function openReportModal(preProjectId=null) {
  REP_FILES = [];
  const sel = document.getElementById('rep-project');
  let projs = STATE.projects;
  if(CU.role==='engineer') {
    const eng = STATE.engineers.find(e=>e.name===CU.name||e.username===CU.username);
    if(eng) projs = projs.filter(p=>p.engineerId===eng.id);
  }
  sel.innerHTML = '<option value="">اختر مشروعاً...</option>'
    + projs.map(p=>`<option value="${p.id}">${esc(p.projectCode)} — ${esc(p.description?.slice(0,30)||'')}</option>`).join('');

  // Pre-select project if provided
  if(preProjectId) {
    sel.value = preProjectId;
    onRepProjChange();
  }

  // Engineer display
  const eng = STATE.engineers.find(e=>e.name===CU.name||e.username===CU.username);
  document.getElementById('rep-engineer-display').value = eng?.name || (CU.role==='manager'?'المدير':'—');

  // Reset fields
  document.getElementById('rep-content').value='';
  document.getElementById('rep-stages').value='';
  document.getElementById('rep-notes').value='';
  document.getElementById('rep-progress').value='0';
  document.getElementById('rep-prog-display').textContent='0';
  document.getElementById('rep-prog-fill').style.width='0%';
  document.getElementById('rep-prog-pct-badge').textContent='0%';
  document.getElementById('rep-file-preview').innerHTML='';
  document.getElementById('rep-char-count').textContent='0 حرف';
  document.getElementById('rep-proj-info').style.display='none';
  document.getElementById('rep-date').value=new Date().toISOString().split('T')[0];

  // Report number preview
  const nextNum = 'RPT-' + String(STATE.reports.length+1).padStart(4,'0');
  document.getElementById('rep-num-preview').textContent = 'رقم التقرير: ' + nextNum;

  document.getElementById('rep-overlay').classList.add('open');
}

function closeRepModal() {
  document.getElementById('rep-overlay').classList.remove('open');
  REP_FILES = [];
}

function onRepProjChange() {
  const id = parseInt(document.getElementById('rep-project').value);
  const p  = STATE.projects.find(pr=>pr.id===id);
  const infoBox = document.getElementById('rep-proj-info');
  const banner  = document.getElementById('rep-proj-banner');
  if(!p) { infoBox.style.display='none'; return; }

  // Sync progress from project
  const prog = p.progress||0;
  document.getElementById('rep-progress').value = prog;
  document.getElementById('rep-prog-display').textContent = prog;
  document.getElementById('rep-prog-fill').style.width = prog+'%';
  document.getElementById('rep-prog-pct-badge').textContent = prog+'%';

  const c = STATE.clients.find(cl=>cl.id===p.clientId);
  const t = TYPES[p.taskTypeKey];
  banner.innerHTML = `
    <div class="eu-info-tag"><i class="ti ti-hash"></i><strong>${esc(p.projectCode)}</strong></div>
    <div class="eu-info-tag"><i class="ti ti-users"></i><span>${esc(c?.name||'—')}</span></div>
    <div class="eu-info-tag"><i class="ti ti-briefcase"></i><span>${t?.icon||''} ${t?.ar||''}</span></div>
    ${p.deliveryDate?`<div class="eu-info-tag"><i class="ti ti-calendar"></i><span>التسليم: ${p.deliveryDate}</span></div>`:''}
    ${p.district?`<div class="eu-info-tag"><i class="ti ti-map-pin"></i><span>${esc(p.district)}</span></div>`:''}`;
  infoBox.style.display='';
}

function updateRepCharCount(el) {
  const n = el.value.length;
  document.getElementById('rep-char-count').textContent = n + ' حرف';
}

// ── File handling ──
function onRepFilesSelected() {
  const inp = document.getElementById('rep-files-inp');
  const MAX = 3 * 1024 * 1024; // 3MB per file for base64 storage
  Array.from(inp.files).forEach(file => {
    if(isImage(file.name) && file.size <= MAX) {
      const reader = new FileReader();
      reader.onload = e => {
        REP_FILES.push({ name:file.name, size:file.size, type:file.type, dataUrl:e.target.result });
        renderRepFilePreview();
      };
      reader.readAsDataURL(file);
    } else {
      REP_FILES.push({ name:file.name, size:file.size, type:file.type, dataUrl:null });
      renderRepFilePreview();
    }
  });
  inp.value='';
}

function renderRepFilePreview() {
  document.getElementById('rep-file-preview').innerHTML = REP_FILES.map((f,i)=>{
    const icon = getFileIcon(f.name);
    const img  = f.dataUrl ? `<img src="${f.dataUrl}" class="img-thumb">` : `<i class="ti ${icon}" style="font-size:16px;color:var(--accent);"></i>`;
    const size = f.size < 1024 ? f.size+'B' : f.size < 1048576 ? Math.round(f.size/1024)+'KB' : Math.round(f.size/1048576*10)/10+'MB';
    return `<div class="rep-form-file-chip">
      ${img}
      <span title="${esc(f.name)}">${esc(f.name.length>20?f.name.slice(0,18)+'…':f.name)}</span>
      <span style="color:var(--text3);font-size:10px;">${size}</span>
      <button onclick="REP_FILES.splice(${i},1);renderRepFilePreview();" style="font-size:11px;padding:2px 8px;"><i class="ti ti-trash" style="font-size:11px;vertical-align:-1px;"></i> حذف</button>
    </div>`;
  }).join('');
  const hint = document.getElementById('rep-save-hint');
  if(hint) hint.textContent = REP_FILES.length
    ? `سيتم حفظ ${REP_FILES.length} مرفق مع التقرير`
    : 'سيتم حفظ التقرير مع جميع المرفقات';
}

// ── Render recent daily reports on dashboard ──
function renderDashRecentLogs() {
  const el = document.getElementById('dash-daily-reports');
  if(!el) return;
  const logs = STATE.reports
    .filter(r=>r.reportType==='daily_site')
    .sort((a,b)=>b.createdAt-a.createdAt)
    .slice(0,5);
  if(!logs.length) {
    el.innerHTML='<div style="color:var(--text3);font-size:12px;padding:8px 0;">لا توجد تقارير يومية بعد</div>';
    return;
  }
  el.innerHTML = logs.map(r=>{
    const dp=(r.date||'').split('-');
    const dd=dp.length===3?dp[2]+'/'+dp[1]:r.date||'—';
    return `<div class="dash-dl-card">
      <div class="dash-dl-date">${dd}</div>
      <div class="dash-dl-body">
        <div class="dash-dl-proj">${esc(r.projectCode||'—')} — <span style="color:var(--text3);font-weight:400;">${esc(r.clientName||'')}</span></div>
        <div class="dash-dl-summary">${esc(r.summary||r.content||'—')}</div>
        <div style="font-size:10.5px;color:var(--text3);margin-top:2px;">
          👷 ${esc(r.engineerName||'—')}${r.workshop?' • 🏭 '+esc(r.workshop):''}${(r.photos||[]).length?' • 📷 '+r.photos.length+' صورة':''}
        </div>
      </div>
      <div style="display:flex;flex-direction:column;gap:5px;flex-shrink:0;">
        <button class="dl-action-btn" style="font-size:11px;padding:5px 9px;" onclick="printDailyReport('${r.logId||r.id}',${r.projectId})"><i class="ti ti-printer"></i> طباعة</button>
        <button class="dl-action-btn" style="font-size:11px;padding:5px 9px;" onclick="openFollowup(${r.projectId})"><i class="ti ti-folder-open"></i> المشروع</button>
      </div>
    </div>`;
  }).join('');
}

// ── Save Report ──
async function saveReport() {
  const projId  = parseInt(document.getElementById('rep-project').value);
  const content = document.getElementById('rep-content').value.trim();
  if(!projId)   { toast('⚠ اختر مشروعاً'); return; }
  if(!content)  { toast('⚠ أكتب محتوى التقرير'); return; }

  const btn = document.getElementById('rep-save-btn');
  if(btn) { btn.disabled=true; btn.textContent='جاري الحفظ...'; }

  const eng = STATE.engineers.find(e=>e.name===CU.name||e.username===CU.username)
    || (CU.role==='manager'?STATE.engineers[0]:null);

  const progVal = parseInt(document.getElementById('rep-progress').value);
  const dateVal = document.getElementById('rep-date').value
    || new Date().toISOString().split('T')[0];

  const report = {
    id:             Date.now(),
    reportNumber:   'RPT-' + String(STATE.reports.length+1).padStart(4,'0'),
    projectId:      projId,
    engineerId:     eng?.id||null,
    reportType:     document.getElementById('rep-type').value,
    content,
    progressSnapshot: isNaN(progVal)?null:progVal,
    stages:         document.getElementById('rep-stages').value.trim(),
    notes:          document.getElementById('rep-notes').value.trim(),
    attachments:    [...REP_FILES], // includes dataUrl for images
    date:           dateVal,
    createdAt:      Date.now()
  };

  await dbPut('reports', report);
  STATE.reports.push(report);

  // Also update project progress if engineer
  const proj = STATE.projects.find(p=>p.id===projId);
  if(proj && report.progressSnapshot != null) {
    proj.progress = report.progressSnapshot;
    proj.updatedAt = Date.now();
    await dbPut('projects', proj);
  }

  closeRepModal();
  renderReports();
  updateBadges();
  toast('✓ تم حفظ التقرير ' + report.reportNumber);
  if(btn) { btn.disabled=false; btn.innerHTML='<i class="ti ti-device-floppy" style="vertical-align:-2px;margin-left:4px;"></i> حفظ التقرير'; }
}

// ── Report Detail ──
function openRepDetail(id) {
  REP_DETAIL_ID = id;
  const r   = STATE.reports.find(x=>x.id===id);
  if(!r) return;
  const proj = STATE.projects.find(p=>p.id===r.projectId);
  const eng  = STATE.engineers.find(e=>e.id===r.engineerId);
  const c    = STATE.clients.find(cl=>cl.id===proj?.clientId);
  const rt   = REP_TYPE_CFG[r.reportType]||{ar:r.reportType,icon:'📄',cls:''};
  const files = r.attachments||[];

  document.getElementById('rd-title').textContent = r.reportNumber||'تقرير';
  document.getElementById('rd-subtitle').textContent =
    (proj?.projectCode||'') + ' — ' + (proj?.description?.slice(0,40)||'');

  // Show delete btn for manager only
  document.getElementById('rd-delete-btn').style.display = CU.role==='manager'?'':'none';

  const imgFiles  = files.filter(f=>isImage(f.name) && f.dataUrl);
  const otherFiles = files.filter(f=>!isImage(f.name) || !f.dataUrl);

  document.getElementById('rd-body').innerHTML = `
    <!-- Meta tags row -->
    <div class="rep-detail-meta">
      <span class="rep-type-badge ${rt.cls}" style="font-size:12px;">${rt.icon} ${rt.ar}</span>
      <div class="rep-detail-tag"><i class="ti ti-hash"></i><strong>${esc(r.reportNumber||'—')}</strong></div>
      <div class="rep-detail-tag"><i class="ti ti-calendar"></i><strong>${r.date||'—'}</strong></div>
      <div class="rep-detail-tag"><i class="ti ti-hard-hat"></i><strong>${esc(eng?.name||'—')}</strong></div>
      ${c?`<div class="rep-detail-tag"><i class="ti ti-users"></i><strong>${esc(c.name)}</strong></div>`:''}
      ${proj?`<div class="rep-detail-tag"><i class="ti ti-folder"></i><strong>${esc(proj.projectCode)}</strong></div>`:''}
    </div>

    <!-- Progress -->
    ${r.progressSnapshot!=null?`
    <div class="rep-detail-section">
      <div class="rep-detail-section-title"><i class="ti ti-chart-bar"></i>لقطة نسبة الإنجاز</div>
      <div style="display:flex;align-items:center;gap:12px;">
        <div class="prog-bar" style="flex:1;height:10px;">
          <div class="prog-fill" style="width:${r.progressSnapshot}%;${r.progressSnapshot===100?'background:var(--green);':''}"></div>
        </div>
        <strong style="font-size:20px;color:var(--accent);min-width:46px;">${r.progressSnapshot}%</strong>
      </div>
    </div>`:''}

    <!-- Content -->
    <div class="rep-detail-section">
      <div class="rep-detail-section-title"><i class="ti ti-file-description"></i>محتوى التقرير</div>
      <div class="rep-detail-content">${esc(r.content||'').replace(/\n/g,'<br>')}</div>
    </div>

    <!-- Stages -->
    ${r.stages?`
    <div class="rep-detail-section">
      <div class="rep-detail-section-title"><i class="ti ti-list-check"></i>مراحل وبنود العمل</div>
      <div class="rep-detail-content" style="border-right-color:var(--project-c);">${esc(r.stages).replace(/\n/g,'<br>')}</div>
    </div>`:''}

    <!-- Notes -->
    ${r.notes?`
    <div class="rep-detail-section">
      <div class="rep-detail-section-title"><i class="ti ti-notes"></i>الملاحظات والتوصيات</div>
      <div class="rep-detail-content" style="border-right-color:var(--amber);">${esc(r.notes).replace(/\n/g,'<br>')}</div>
    </div>`:''}

    <!-- Image attachments -->
    ${imgFiles.length?`
    <div class="rep-detail-section">
      <div class="rep-detail-section-title"><i class="ti ti-photo"></i>الصور المرفقة (${imgFiles.length})</div>
      <div style="display:flex;flex-wrap:wrap;gap:8px;">
        ${imgFiles.map(f=>`<a href="${f.dataUrl}" download="${esc(f.name)}" title="${esc(f.name)}">
          <img src="${f.dataUrl}" class="rep-att-img-preview" alt="${esc(f.name)}">
        </a>`).join('')}
      </div>
    </div>`:''}

    <!-- Other file attachments -->
    ${otherFiles.length?`
    <div class="rep-detail-section">
      <div class="rep-detail-section-title"><i class="ti ti-paperclip"></i>الملفات المرفقة (${otherFiles.length})</div>
      <div class="rep-detail-attachments">
        ${otherFiles.map(f=>`<div class="rep-att-chip">
          <i class="ti ${getFileIcon(f.name)}" style="font-size:18px;"></i>
          <span>${esc(f.name)}</span>
          ${f.size?`<span style="font-size:10px;color:var(--text3);">${f.size<1048576?Math.round(f.size/1024)+'KB':Math.round(f.size/1048576*10)/10+'MB'}</span>`:''}
        </div>`).join('')}
      </div>
    </div>`:''}

    ${!files.length?`<div style="font-size:12px;color:var(--text3);text-align:center;padding:8px 0;">لا توجد مرفقات</div>`:''}

    <div style="font-size:11px;color:var(--text3);text-align:center;padding-top:4px;border-top:1px solid var(--border);">
      أُنشئ في: ${fmtDate(r.createdAt)}
    </div>`;

  document.getElementById('rep-detail-overlay').classList.add('open');
}

function closeRepDetail() {
  document.getElementById('rep-detail-overlay').classList.remove('open');
  REP_DETAIL_ID = null;
}

async function deleteReportConfirm() {
  if(!REP_DETAIL_ID) return;
  if(!confirm('حذف هذا التقرير نهائياً؟')) return;
  await dbDelete('reports', REP_DETAIL_ID);
  STATE.reports = STATE.reports.filter(r=>r.id!==REP_DETAIL_ID);
  closeRepDetail();
  renderReports();
  toast('تم حذف التقرير');
}

function printReport() {
  const r   = STATE.reports.find(x=>x.id===REP_DETAIL_ID);
  if(!r) return;
  const proj = STATE.projects.find(p=>p.id===r.projectId);
  const eng  = STATE.engineers.find(e=>e.id===r.engineerId);
  const c    = STATE.clients.find(cl=>cl.id===proj?.clientId);
  const rt   = REP_TYPE_CFG[r.reportType]||{ar:r.reportType,icon:'📄'};
  const files= (r.attachments||[]).filter(f=>isImage(f.name)&&f.dataUrl);
  const w = window.open('','_blank','width=794,height=1123');
  w.document.write(`<!DOCTYPE html><html dir="rtl" lang="ar"><head>
    <meta charset="UTF-8"><title>${r.reportNumber}</title>
    <style>
      body{font-family:'Segoe UI',Tahoma,Arial,sans-serif;padding:40px;color:#1C1C1A;direction:rtl;font-size:13px;}
      h1{font-size:20px;margin-bottom:4px;}
      .meta{display:flex;gap:16px;flex-wrap:wrap;color:#666;font-size:11px;border-bottom:2px solid #534AB7;padding-bottom:10px;margin-bottom:18px;}
      .section{margin-bottom:16px;}
      .section-title{font-size:11px;font-weight:700;color:#9A9A94;text-transform:uppercase;margin-bottom:6px;}
      .box{background:#F7F6F3;padding:12px;border-radius:6px;line-height:1.7;border-right:3px solid #534AB7;}
      .prog-wrap{display:flex;align-items:center;gap:12px;}
      .prog-bar{flex:1;height:10px;background:#EEEDEA;border-radius:5px;overflow:hidden;}
      .prog-fill{height:100%;background:linear-gradient(90deg,#534AB7,#AFA9EC);}
      .imgs{display:flex;flex-wrap:wrap;gap:8px;margin-top:6px;}
      .imgs img{width:140px;height:100px;object-fit:cover;border-radius:6px;border:1px solid #ddd;}
      @media print{body{padding:20px;}}
    </style>
  </head><body>
    <h1>${r.reportNumber} — ${rt.icon} ${rt.ar}</h1>
    <div class="meta">
      <span>المشروع: <strong>${proj?.projectCode||'—'}</strong></span>
      <span>العميل: <strong>${c?.name||'—'}</strong></span>
      <span>المهندس: <strong>${eng?.name||'—'}</strong></span>
      <span>التاريخ: <strong>${r.date||'—'}</strong></span>
    </div>
    ${r.progressSnapshot!=null?`<div class="section"><div class="section-title">نسبة الإنجاز</div>
      <div class="prog-wrap"><div class="prog-bar"><div class="prog-fill" style="width:${r.progressSnapshot}%"></div></div><strong>${r.progressSnapshot}%</strong></div></div>`:''}
    <div class="section"><div class="section-title">محتوى التقرير</div>
      <div class="box">${(r.content||'').replace(/</g,'&lt;').replace(/>/g,'&gt;').replace(/\n/g,'<br>')}</div></div>
    ${r.stages?`<div class="section"><div class="section-title">المراحل المنجزة</div>
      <div class="box">${r.stages.replace(/</g,'&lt;').replace(/>/g,'&gt;').replace(/\n/g,'<br>')}</div></div>`:''}
    ${r.notes?`<div class="section"><div class="section-title">الملاحظات</div>
      <div class="box">${r.notes.replace(/</g,'&lt;').replace(/>/g,'&gt;').replace(/\n/g,'<br>')}</div></div>`:''}
    ${files.length?`<div class="section"><div class="section-title">الصور المرفقة</div>
      <div class="imgs">${files.map(f=>`<img src="${f.dataUrl}" alt="${f.name}">`).join('')}</div></div>`:''}
  
<script>
// ── Startup: check session then show login or app ──
(async function startApp() {
  await initDB();
  // Load dynamic users first
  try {
    const uSaved = localStorage.getItem('pxid_users');
    DUSERS = uSaved ? JSON.parse(uSaved) : null;
  } catch(e) { DUSERS = null; }

  const restored = tryRestoreSession();
  if (restored) {
    // Valid session — go straight to app
    await loadAllData();
    document.getElementById('login-wrap').style.display = 'none';
    document.getElementById('app').style.display = 'flex';
    applyRoleUI();
    renderAll();
  } else {
    // No session — show login
    document.getElementById('login-wrap').style.display = 'flex';
    document.getElementById('app').style.display = 'none';
  }
})();
</script>
</body></html>`);
  w.document.close();
  setTimeout(()=>w.print(),500);
}

// ══════════════════════════════════════════════════════════════════
// SETTINGS / ENGINEERS
// ══════════════════════════════════════════════════════════════════
function renderSettings() {
  if(CU?.role==='engineer') return;
  const el = document.getElementById('eng-list');
  if(!el) return;
  el.innerHTML = STATE.engineers.map(e=>`
    <div style="display:flex;align-items:center;gap:12px;padding:10px 0;border-bottom:1px solid var(--border);">
      <div style="width:36px;height:36px;border-radius:50%;background:var(--accent);display:flex;align-items:center;justify-content:center;color:#fff;font-weight:700;font-size:13px;flex-shrink:0;">${e.name.charAt(0)}</div>
      <div style="flex:1;">
        <div style="font-size:13px;font-weight:600;">${esc(e.name)}</div>
        <div style="font-size:11px;color:var(--text3);">${esc(e.phone||'')} ${e.email?'• '+esc(e.email):''}</div>
      </div>
      <button class="icon-btn del" onclick="deleteEngineer(${e.id})"><i class="ti ti-trash"></i> حذف</button>
    </div>`).join('');
}

function openAddEngineer() { document.getElementById('eng-modal').classList.add('open'); }
function closeEngModal() { document.getElementById('eng-modal').classList.remove('open'); }

async function saveEngineer() {
  const name = document.getElementById('eng-name').value.trim();
  if(!name) { toast('أدخل اسم المهندس'); return; }
  const eng = {
    id: Date.now(),
    name,
    phone: document.getElementById('eng-phone').value.trim(),
    whatsapp: document.getElementById('eng-wa').value.trim(),
    email: document.getElementById('eng-email').value.trim(),
    createdAt: Date.now()
  };
  await dbPut('engineers', eng);
  STATE.engineers.push(eng);
  closeEngModal();
  renderSettings();
  toast('✓ تم إضافة المهندس');
}

async function deleteEngineer(id) {
  if(!confirm('حذف هذا المهندس؟')) return;
  await dbDelete('engineers', id);
  STATE.engineers = STATE.engineers.filter(e=>e.id!==id);
  renderSettings();
  toast('تم حذف المهندس');
}

function exportData() {
  const data = {clients:STATE.clients,projects:STATE.projects,engineers:STATE.engineers,reports:STATE.reports,exportedAt:new Date().toISOString()};
  const blob = new Blob([JSON.stringify(data,null,2)],{type:'application/json'});
  const a = document.createElement('a');
  a.href = URL.createObjectURL(blob);
  a.download = 'projexid_export_'+new Date().toISOString().split('T')[0]+'.json';
  a.click();
}

async function clearAll() {
  if (!DB) await initDB();
  for(const s of ['clients','projects','engineers','reports']) {
    const tx = DB.transaction(s,'readwrite');
    tx.objectStore(s).clear();
  }
  STATE.clients=[];STATE.projects=[];STATE.reports=[];
  STATE.engineers=[{id:1001,name:'أحمد الرشيدي',phone:'+966501234567',whatsapp:'+966501234567',email:'ahmed@example.com',createdAt:Date.now()},{id:1002,name:'سارة المحمود',phone:'+966502345678',whatsapp:'+966502345678',email:'',createdAt:Date.now()}];
  for(const e of STATE.engineers) await dbPut('engineers',e);
  renderAll();
  toast('تم مسح البيانات');
}

// ══════════════════════════════════════════════════════════════════
// WORK ORDER MODAL
// ══════════════════════════════════════════════════════════════════
function openWorkOrder() {
  try {
    WO_EDIT_ID = null;
    WO_FILES = [];
    WO_PAYMENTS = [];

    // إعادة تعيين الحقول بأمان
    const setVal = (id, val) => { const el = document.getElementById(id); if(el) el.value = val; };
    const setHTML = (id, val) => { const el = document.getElementById(id); if(el) el.innerHTML = val; };
    const setDisp = (id, val) => { const el = document.getElementById(id); if(el) el.style.display = val; };
    const setText = (id, val) => { const el = document.getElementById(id); if(el) el.textContent = val; };

    setText('wo-title', 'أمر عمل جديد');
    setVal('wo-client', '');
    setVal('wo-client-code', '');
    setVal('wo-type', 'design');
    setVal('wo-proj-code', '');
    setVal('wo-desc', '');
    setVal('wo-prop-num', '');
    setVal('wo-district', '');
    setVal('wo-total', '');
    setVal('wo-currency', 'USD');
    setVal('wo-pri', 'medium');
    setVal('wo-recv-date', new Date().toISOString().split('T')[0]);
    setVal('wo-del-date', '');
    setVal('wo-status', 'waiting');
    setVal('wo-engineer-name', '');
    setVal('wo-engineer-id', '');
    setVal('wo-eng-wa', '');
    setHTML('wo-file-list', '');
    setDisp('new-client-fields', 'none');

    populateWOSelects();
    onTypeChange();

    const overlay = document.getElementById('wo-overlay');
    if(overlay) {
      overlay.classList.add('open');
    } else {
      toast('⚠ خطأ: لم يتم العثور على النافذة');
    }
  } catch(e) {
    console.error('openWorkOrder error:', e);
    toast('⚠ خطأ في فتح النافذة: ' + e.message);
  }
}

// ── Mobile nav sync (patched here after sw() is defined) ──
const _origSw = window.sw || sw;
window.sw = function(view, el) {
  _origSw(view, el);
  if (typeof mbnActivate === 'function') mbnActivate(view);
  if (typeof closeMoreDrawer === 'function') closeMoreDrawer();
};

function openEditWO(id) {
  const p = STATE.projects.find(pr=>pr.id===id);
  if(!p) return;
  WO_EDIT_ID = id;
  WO_FILES = [];
  const wCurrency = p.currency||'USD';
  document.getElementById('wo-currency').value = wCurrency;
  // WO payments
  const storedWOPay = JSON.parse(JSON.stringify(p.payments||[]));
  WO_PAYMENTS = storedWOPay.map(pp=>({ label: pp.label, status: pp.status, amount: pp.amount||0 }));
  document.getElementById('wo-title').textContent = 'تعديل أمر العمل — ' + p.projectCode;
  populateWOSelects();

  document.getElementById('wo-client').value = p.clientId||'';
  onClientChange(true);
  document.getElementById('wo-type').value = p.taskTypeKey||'design';
  onTypeChange(true);
  document.getElementById('wo-proj-code').value = p.projectCode||'';
  document.getElementById('wo-desc').value = p.description||'';
  document.getElementById('wo-prop-num').value = p.propertyNumber||'';
  document.getElementById('wo-district').value = p.district||'';
  document.getElementById('wo-total').value = p.totalAmount||'';
  document.getElementById('wo-pri').value = p.priority||'medium';
  document.getElementById('wo-recv-date').value = p.receivedDate||'';
  document.getElementById('wo-del-date').value = p.deliveryDate||'';
  document.getElementById('wo-status').value = p.status||'waiting';
  const engineer = STATE.engineers.find(en=>en.id===p.engineerId);
  document.getElementById('wo-engineer-name').value = engineer ? engineer.name : (p.engineerName||'');
  document.getElementById('wo-engineer-id').value = p.engineerId||'';
  onEngineerNameChange();
  document.getElementById('wo-file-list').innerHTML='';
  document.getElementById('wo-overlay').classList.add('open');
}

function closeWO() { document.getElementById('wo-overlay').classList.remove('open'); }

function populateWOSelects() {
  // Clients
  const csel = document.getElementById('wo-client');
  csel.innerHTML = '<option value="">اختر عميلاً...</option>' + STATE.clients.map(c=>`<option value="${c.id}">${esc(c.name)} (${esc(c.clientCode)})</option>`).join('') + '<option value="NEW">+ عميل جديد</option>';
  // Engineers
  const engInput = document.getElementById('wo-engineer-name');
  const engList = document.getElementById('wo-engineer-list');
  engInput.value = '';
  document.getElementById('wo-engineer-id').value = '';
  engList.innerHTML = STATE.engineers.map(e=>`<option value="${esc(e.name)}"></option>`).join('');
}

function onClientChange(silent=false) {
  const val = document.getElementById('wo-client').value;
  const nf = document.getElementById('new-client-fields');
  if(val==='NEW') {
    nf.style.display='';
    document.getElementById('wo-client-code').value='';
    return;
  }
  nf.style.display='none';
  const c = STATE.clients.find(cl=>String(cl.id)===val);
  document.getElementById('wo-client-code').value = c?c.clientCode:'';
}

function onTypeChange(silent=false) {
  if(WO_EDIT_ID&&silent) return;
  const t = document.getElementById('wo-type').value;
  const info = TYPES[t];
  if(!info) return;
  const count = STATE.projects.filter(p=>p.taskTypeKey===t).length+1;
  const code = info.prefix + '-' + String(count).padStart(3,'0');
  document.getElementById('wo-proj-code').value = code;
}

function onEngineerNameChange() {
  const name = document.getElementById('wo-engineer-name').value.trim();
  const e = STATE.engineers.find(en=>en.name===name);
  if (e) {
    document.getElementById('wo-engineer-id').value = e.id;
    document.getElementById('wo-eng-wa').value = e.whatsapp||e.phone||'';
  } else {
    document.getElementById('wo-engineer-id').value = '';
    document.getElementById('wo-eng-wa').value = '';
  }
}

function onFilesSelected() {
  const inp = document.getElementById('wo-files-inp');
  for(const f of inp.files) WO_FILES.push({name:f.name,size:f.size,type:f.type});
  renderWOFileList();
  inp.value='';
}

function renderWOFileList() {
  document.getElementById('wo-file-list').innerHTML = WO_FILES.map((f,i)=>`
    <div class="file-chip">${esc(f.name)}<button onclick="WO_FILES.splice(${i},1);renderWOFileList();" style="font-size:11px;padding:2px 8px;"><i class="ti ti-trash" style="font-size:11px;vertical-align:-1px;"></i> حذف</button></div>`).join('');
}

function addPayment() { /* payment list removed */ }

function renderWOPayments() { /* payment list removed */ }

function calcPayments() { /* payment list removed */ }

async function saveWO() {
  const name = document.getElementById('wo-client').value;
  const type = document.getElementById('wo-type').value;
  const desc = document.getElementById('wo-desc').value.trim();
  if(!type) { toast('أكمل الحقول المطلوبة'); return; }

  let clientId;
  if(name==='NEW'||!name) {
    // create new client
    const cn = document.getElementById('wo-new-client-name').value.trim();
    const ph = document.getElementById('wo-new-client-phone').value.trim();
    if(!cn||!ph) { toast('أدخل اسم ورقم هاتف العميل'); return; }
    if(STATE.clients.find(c=>c.name===cn)) { toast('العميل موجود مسبقاً'); return; }
    const cid = Date.now();
    const num = STATE.clients.length+1;
    const nc = { id:cid, name:cn, clientCode:'CLIENT #'+String(num).padStart(3,'0'), phone:ph, email:document.getElementById('wo-new-client-email').value.trim(), finance:{totalAmount:0,payments:[]}, createdAt:Date.now() };
    await dbPut('clients', nc);
    STATE.clients.push(nc);
    clientId = cid;
  } else {
    clientId = parseInt(name);
  }

  let engineerId = parseInt(document.getElementById('wo-engineer-id').value) || null;
  const engineerName = document.getElementById('wo-engineer-name').value.trim();
  if (!engineerId && engineerName) {
    const existing = STATE.engineers.find(en=>en.name===engineerName);
    if (existing) {
      engineerId = existing.id;
      document.getElementById('wo-engineer-id').value = engineerId;
    } else {
      const newEng = { id: Date.now(), name: engineerName, phone:'', whatsapp:'', email:'', createdAt: Date.now() };
      await dbPut('engineers', newEng);
      STATE.engineers.push(newEng);
      engineerId = newEng.id;
      populateWOSelects();
      document.getElementById('wo-engineer-name').value = engineerName;
      document.getElementById('wo-engineer-id').value = engineerId;
      onEngineerNameChange();
    }
  }

  const code = document.getElementById('wo-proj-code').value;
  const info = TYPES[type];

  const proj = {
    id: WO_EDIT_ID||Date.now(),
    projectCode: code,
    taskTypeArabic: info.ar,
    taskTypeEnglish: type,
    taskTypeKey: type,
    clientId,
    description: desc,
    propertyNumber: document.getElementById('wo-prop-num').value.trim(),
    district: document.getElementById('wo-district').value.trim(),
    attachments: WO_FILES,
    // store values as entered
    totalAmount: parseFloat(document.getElementById('wo-total').value)||0,
    payments: [],
    currency: document.getElementById('wo-currency')?.value||'USD',
    priority: document.getElementById('wo-pri').value,
    receivedDate: document.getElementById('wo-recv-date').value,
    deliveryDate: document.getElementById('wo-del-date').value,
    engineerId: parseInt(document.getElementById('wo-engineer-id').value)||null,
    engineerName: document.getElementById('wo-engineer-name').value.trim() || null,
    status: document.getElementById('wo-status').value,
    createdAt: WO_EDIT_ID?(STATE.projects.find(p=>p.id===WO_EDIT_ID)?.createdAt||Date.now()):Date.now(),
    updatedAt: Date.now()
  };

  // ── Sync Work Order → Finance Statement (fin2) ──────────────────
  {
    // Preserve existing fin2 on edit, create fresh for new project
    const oldProj = WO_EDIT_ID ? STATE.projects.find(p=>p.id===WO_EDIT_ID) : null;
    const existingFin2 = oldProj?.fin2 ? JSON.parse(JSON.stringify(oldProj.fin2)) : null;
    const fin2 = existingFin2 || { contractAmount: 0, currency: 'USD', payments: [], expenses: [] };
    if (!fin2.payments) fin2.payments = [];
    if (!fin2.expenses) fin2.expenses = [];

    // 1. Sync contract amount and currency as entered
    fin2.contractAmount = proj.totalAmount;   // stored as entered
    fin2.currency       = proj.currency || 'USD';  // currency as entered

    // 2. Sync paid WO payments → remove previous WO-sourced entries, re-add current paid ones
    //    (so editing the WO always reflects the latest payment status)
    fin2.payments = fin2.payments.filter(pm => pm.source !== 'workorder');
    const woRecvDate = proj.receivedDate || new Date().toISOString().split('T')[0];
    const woCur      = proj.currency || 'USD';

    // Payments registered separately via Finance section

    proj.fin2 = fin2;
  }
  // ─────────────────────────────────────────────────────────────────

  await dbPut('projects', proj);
  if(WO_EDIT_ID) {
    const idx = STATE.projects.findIndex(p=>p.id===WO_EDIT_ID);
    if(idx!==-1) STATE.projects[idx]=proj; else STATE.projects.push(proj);
  } else {
    STATE.projects.unshift(proj);
  }

  // Legacy sync
  if(proj.totalAmount) {
    const c = STATE.clients.find(cl=>cl.id===clientId);
    if(c) { if(!c.finance) c.finance={totalAmount:0,payments:[]}; c.finance.totalAmount=proj.totalAmount; c.finance.payments=proj.payments; await dbPut('clients',c); }
  }

  closeWO();
  renderProjects();
  renderDashboard();
  renderClients();
  updateBadges();
  notifyEngineerAssignment(proj);
  logActivity(WO_EDIT_ID?'تعديل مشروع':'إضافة مشروع جديد', proj.projectCode);
  toast(WO_EDIT_ID?'✓ تم تحديث أمر العمل':'✓ تم إضافة أمر العمل');
}

// ── Notify assigned engineer via WhatsApp + Email ──
function notifyEngineerAssignment(proj) {
  if(!proj || !proj.engineerId) return;
  const eng = STATE.engineers.find(e=>e.id===proj.engineerId);
  if(!eng) return;
  const client = STATE.clients.find(c=>c.id===proj.clientId);
  const typeAr = (TYPES[proj.taskTypeKey]?.ar) || proj.taskTypeArabic || '';
  const lines = [
    `مرحباً ${eng.name},`,
    `تم إسناد مهمة جديدة إليك:`,
    `• رقم المشروع: ${proj.projectCode}`,
    `• نوع المهمة: ${typeAr}`,
    client ? `• العميل: ${client.name}` : '',
    proj.description ? `• الوصف: ${proj.description}` : '',
    proj.deliveryDate ? `• تاريخ التسليم: ${proj.deliveryDate}` : '',
    `• الأولوية: ${proj.priority||'-'}`,
    '',
    `🔗 رابط الموقع: ${window.location.origin + window.location.pathname}`,
  ].filter(Boolean);
  const msg = lines.join('\n');

  // WhatsApp (wa.me)
  const waRaw = (eng.whatsapp || eng.phone || '').replace(/[^\d]/g,'');
  if(waRaw) {
    const waUrl = `https://wa.me/${waRaw}?text=${encodeURIComponent(msg)}`;
    window.open(waUrl, '_blank', 'noopener');
  }
  // Email (mailto)
  if(eng.email) {
    const subject = `مهمة جديدة — ${proj.projectCode}`;
    const mailUrl = `mailto:${encodeURIComponent(eng.email)}?subject=${encodeURIComponent(subject)}&body=${encodeURIComponent(msg)}`;
    setTimeout(()=>window.open(mailUrl, '_blank', 'noopener'), 300);
  }
  if(waRaw || eng.email) {
    toast('✓ تم فتح إشعار المهندس عبر '+([waRaw?'واتساب':'', eng.email?'البريد':''].filter(Boolean).join(' و')));
  }
}

// ═══ WORKFORCE PAYMENTS ══════════════════════════════════════════
let WF_PAY_ENTITY_ID = null; // current worker or workshop id
let WF_PAY_TYPE = null;      // 'worker' | 'workshop'

function fuWkPayOpen(id) {
  WF_PAY_ENTITY_ID = id; WF_PAY_TYPE = 'worker';
  const p = STATE.projects.find(x=>x.id===FU_CUR);
  const w = (p?.workforce?.workers||[]).find(x=>x.id===id);
  if(!w) return;
  const fin = getProjFin(p);
  const cur = fin.currency || p.currency || 'USD';
  const total = wkTotal(w), paid = wkPaid(w);
  document.getElementById('wf-pay-title').textContent = `دفعة للعامل: ${w.name||'—'}`;
  document.getElementById('wf-pay-info').textContent  =
    `الإجمالي: ${fmt(total,cur)} | المدفوع: ${fmt(paid,cur)} | المتبقي: ${fmt(total-paid,cur)}`;
  document.getElementById('wf-pay-type-row').style.display = 'none'; // workers: no type needed
  document.getElementById('wf-pay-amount').value = '';
  document.getElementById('wf-pay-date').value   = new Date().toISOString().split('T')[0];
  document.getElementById('wf-pay-method').value = '';
  document.getElementById('wf-pay-ref').value    = '';
  document.getElementById('wf-pay-notes').value  = '';
  document.getElementById('wf-pay-overlay').classList.add('open');
}

function fuSpPayOpen(id) {
  WF_PAY_ENTITY_ID = id; WF_PAY_TYPE = 'workshop';
  const p  = STATE.projects.find(x=>x.id===FU_CUR);
  const s  = (p?.workforce?.workshops||[]).find(x=>x.id===id);
  if(!s) return;
  const fin = getProjFin(p);
  const cur = fin.currency || p.currency || 'USD';
  const total = spTotal(s), paid = spPaid(s);
  document.getElementById('wf-pay-title').textContent = `دفعة للورشة: ${s.name||'—'}`;
  document.getElementById('wf-pay-info').textContent  =
    `قيمة العقد: ${fmt(total,cur)} | المدفوع: ${fmt(paid,cur)} | المتبقي: ${fmt(total-paid,cur)}`;
  document.getElementById('wf-pay-type-row').style.display = '';
  document.getElementById('wf-pay-pay-type').value = 'advance';
  document.getElementById('wf-pay-amount').value = '';
  document.getElementById('wf-pay-date').value   = new Date().toISOString().split('T')[0];
  document.getElementById('wf-pay-method').value = '';
  document.getElementById('wf-pay-ref').value    = '';
  document.getElementById('wf-pay-notes').value  = '';
  document.getElementById('wf-pay-overlay').classList.add('open');
}

async function fuWfPaySave() {
  const amount = parseFloat(document.getElementById('wf-pay-amount').value)||0;
  const date   = document.getElementById('wf-pay-date').value;
  if (!amount) { toast('⚠ أدخل المبلغ'); return; }
  if (!date)   { toast('⚠ أدخل التاريخ'); return; }
  const p = STATE.projects.find(x=>x.id===FU_CUR);
  if (!p) return;
  const payment = {
    id:     fuUID('pm'),
    amount, date,
    type:   document.getElementById('wf-pay-pay-type').value || 'advance',
    method: document.getElementById('wf-pay-method').value,
    ref:    document.getElementById('wf-pay-ref').value,
    notes:  document.getElementById('wf-pay-notes').value.trim(),
  };
  if (WF_PAY_TYPE === 'worker') {
    const w = (p.workforce.workers||[]).find(x=>x.id===WF_PAY_ENTITY_ID);
    if (!w) return;
    if (!w.payments) w.payments=[];
    w.payments.push(payment);
  } else {
    const s = (p.workforce.workshops||[]).find(x=>x.id===WF_PAY_ENTITY_ID);
    if (!s) return;
    if (!s.payments) s.payments=[];
    s.payments.push(payment);
  }
  await fuSave();
  document.getElementById('wf-pay-overlay').classList.remove('open');
  fuRender();
  wfSyncFinance();
  toast(`✓ تم تسجيل الدفعة`);
}
// ═══ DAILY SITE LOG — NEW FUNCTIONS ════════════════════════════

function fuLogGetWorkshops() {
  // Get workshop names from current project + standard types
  const p = STATE.projects.find(x=>x.id===FU_CUR);
  const wsNames = (p?.workforce?.workshops||[]).map(s=>s.name||s.type).filter(Boolean);
  const defaults = ['ورشة حدادة','ورشة بناء','ورشة كهرباء','ورشة سباكة',
                    'ورشة لياسة','ورشة سيراميك','ورشة دهانات','ورشة نجارة','ورشة تكييف'];
  return [...new Set([...wsNames, ...defaults])];
}

async function fuLogSubmit(logId) {
  const p = STATE.projects.find(x=>x.id===FU_CUR);
  if(!p) { toast('⚠ خطأ: لم يتم تحديد المشروع'); return; }
  const log = (p.tracking.dailyLogs||[]).find(L=>L.id===logId);
  if(!log) { toast('⚠ خطأ: لم يتم العثور على السجل'); return; }
  if(!log.work && !log.notes && !log.summary) {
    toast('⚠ أدخل تفاصيل الأعمال أو ملخص قبل الإرسال'); return;
  }

  try {
    // Auto-generate summary if empty
    if(!log.summary) log.summary = (log.work||log.notes||'').slice(0,150);
    log.status      = 'submitted';
    log.submittedAt = Date.now();
    log.submittedBy = CU.name || 'المهندس';

    // Save updated project (with submitted log)
    await fuSave();

    // Build the report object — use numeric id for IDB compatibility
    const repId  = Date.now();                // numeric id
    const eng    = STATE.engineers.find(e=>e.name===CU.name||e.username===CU.username);
    const c      = STATE.clients.find(cl=>cl.id===p.clientId);
    const t      = TYPES[p.taskTypeKey]||{};

    const report = {
      id:           repId,               // numeric → IDB safe
      reportType:   'daily_site',
      logId:        logId,               // reference to source log
      projectId:    p.id,
      projectCode:  p.projectCode,
      projectName:  p.description || p.projectCode,
      clientName:   c?.name || '',
      engineerId:   eng?.id || null,
      engineerName: CU.name || log.submittedBy || '',
      taskTypeName: t.ar || '',
      date:         log.date,
      reportTime:   new Date().toLocaleTimeString('ar-SA'),
      createdAt:    repId,
      title:        'سجل يومي — ' + p.projectCode + ' — ' + log.date,
      summary:      log.summary,
      workshop:     log.workshop || '',
      content:      log.work    || '',
      notes:        log.notes   || '',
      incidents:    log.incidents || '',
      materials:    log.materials || '',
      photos:       log.photos  || [],
      issues:       log.issues  || [],
      reportStatus: 'submitted',
      status:       'مُرسَل',
      workersCount: log.workersCount || 0,
    };

    // Update STATE.reports in-memory (remove duplicates for same log, add new)
    STATE.reports = (STATE.reports||[]).filter(r => r.logId !== logId);
    STATE.reports.unshift(report);

    // Persist to IndexedDB
    await dbPut('reports', report);

    // Re-render followup (log now shows as submitted)
    fuRender();

    // Force reports section to update regardless of whether it's visible
    renderReports();
    renderDashboard();
    if(typeof renderDashRecentLogs==='function') renderDashRecentLogs();

    toast('✓ تم إرسال التقرير — يظهر الآن في قسم التقارير');

  } catch(err) {
    console.error('fuLogSubmit error:', err);
    toast('⚠ حدث خطأ أثناء الإرسال — تحقق من وحدة التحكم');
  }
}

async function fuLogIssueAdd(logId) {
  const p = STATE.projects.find(x=>x.id===FU_CUR); if(!p) return;
  const log = (p.tracking.dailyLogs||[]).find(L=>L.id===logId); if(!log) return;
  if(!log.issues) log.issues=[];
  log.issues.push({
    id:'ISS'+Date.now(), description:'', workshop:'',
    priority:'متوسطة', status:'مفتوحة',
    createdAt:Date.now(), resolveBy:''
  });
  await fuSave(); fuRender();
}
async function fuLogIssueField(logId, idx, k, v) {
  const p = STATE.projects.find(x=>x.id===FU_CUR); if(!p) return;
  const log = (p.tracking.dailyLogs||[]).find(L=>L.id===logId); if(!log) return;
  if(log.issues[idx]) log.issues[idx][k]=v;
  await fuSave();
}
async function fuLogIssueDel(logId, idx) {
  const p = STATE.projects.find(x=>x.id===FU_CUR); if(!p) return;
  const log = (p.tracking.dailyLogs||[]).find(L=>L.id===logId); if(!log) return;
  log.issues.splice(idx,1);
  await fuSave(); fuRender();
}

// Print a daily report
function printDailyReport(logOrRepId, projId) {
  // Find report from STATE.reports or reconstruct from log
  let rep = STATE.reports.find(r=>r.logId===logOrRepId||r.id===logOrRepId);
  if(!rep && projId) {
    const p = STATE.projects.find(x=>x.id==projId);
    const log = (p?.tracking?.dailyLogs||[]).find(L=>L.id===logOrRepId);
    if(log && p) {
      const c = STATE.clients.find(cl=>cl.id===p.clientId);
      rep = { projectCode:p.projectCode, clientName:c?.name||'', engineerName:log.submittedBy||CU.name,
              date:log.date, summary:log.summary, content:log.work, notes:log.notes,
              incidents:log.incidents, materials:log.materials, photos:log.photos||[],
              issues:log.issues||[], workersCount:log.workersCount, workshop:log.workshop };
    }
  }
  if(!rep) { toast('⚠ لم يتم العثور على التقرير'); return; }
  const photoHtml = (rep.photos||[]).map(ph=>`<img src="${ph}" style="height:120px;border-radius:6px;margin:4px;border:1px solid #ddd;">`).join('');
  const issueRows = (rep.issues||[]).map((iss,i)=>`<tr><td>${i+1}</td><td>${esc(iss.description||'')}</td><td>${esc(iss.workshop||'—')}</td><td>${esc(iss.priority||'')}</td><td>${esc(iss.status||'')}</td><td>${iss.resolveBy||'—'}</td></tr>`).join('');
  const w = window.open('','_blank','width=860,height:1200');
  w.document.write(`<!DOCTYPE html><html dir="rtl" lang="ar"><head><meta charset="UTF-8">
    <title>تقرير يومي — ${esc(rep.projectCode||'')}</title>
    <style>body{font-family:'Segoe UI',Tahoma,sans-serif;padding:30px;direction:rtl;color:#1c1c1a;}
    h1{font-size:20px;margin:0 0 4px;}h2{font-size:14px;color:#534AB7;border-bottom:2px solid #534AB7;padding-bottom:4px;margin:16px 0 8px;}
    .meta{display:grid;grid-template-columns:repeat(3,1fr);gap:8px;background:#f5f5f5;padding:12px;border-radius:8px;margin:12px 0;}
    .meta-item{font-size:12px;}.meta-lbl{color:#666;font-size:10px;}
    table{width:100%;border-collapse:collapse;font-size:12px;}th,td{border:1px solid #e5e7eb;padding:7px 10px;text-align:right;}
    th{background:#f3f4f6;}p{font-size:13px;line-height:1.7;color:#444;}
    @media print{body{padding:15px;}}</style>
  </head><body>
    <h1>📅 تقرير يومي للموقع</h1>
    <p style="color:#666;margin:0 0 10px;">مشروع: <strong>${esc(rep.projectCode||'')}</strong> — عميل: ${esc(rep.clientName||'—')}</p>
    <div class="meta">
      <div class="meta-item"><div class="meta-lbl">التاريخ</div><strong>${rep.date||'—'}</strong></div>
      <div class="meta-item"><div class="meta-lbl">المهندس</div><strong>${esc(rep.engineerName||'—')}</strong></div>
      <div class="meta-item"><div class="meta-lbl">الورشة</div><strong>${esc(rep.workshop||'—')}</strong></div>
      <div class="meta-item"><div class="meta-lbl">عدد العمال</div><strong>${rep.workersCount||0}</strong></div>
      <div class="meta-item"><div class="meta-lbl">الحالة</div><strong>${esc(rep.status||'مُرسَل')}</strong></div>
      <div class="meta-item"><div class="meta-lbl">الصور</div><strong>${(rep.photos||[]).length} صورة</strong></div>
    </div>
    <h2>الملخص</h2><p>${esc(rep.summary||'—')}</p>
    <h2>الأعمال المنفذة</h2><p>${esc(rep.content||'—')}</p>
    ${rep.materials?`<h2>المواد المستخدمة</h2><p>${esc(rep.materials)}</p>`:''}
    ${rep.incidents?`<h2>الحوادث والمشاكل</h2><p>${esc(rep.incidents)}</p>`:''}
    ${rep.notes?`<h2>الملاحظات</h2><p>${esc(rep.notes)}</p>`:''}
    ${issueRows?`<h2>المشاكل الميدانية</h2><table><thead><tr><th>#</th><th>المشكلة</th><th>الورشة</th><th>الأولوية</th><th>الحالة</th><th>موعد المعالجة</th></tr></thead><tbody>${issueRows}</tbody></table>`:''}
    ${photoHtml?`<h2>الصور</h2><div>${photoHtml}</div>`:''}
    <hr style="margin-top:30px;"><p style="font-size:10px;color:#999;">طُبع من ProjexID — ${new Date().toLocaleString('ar-SA')}</p>
  
<script>
// ── Startup: check session then show login or app ──
(async function startApp() {
  await initDB();
  // Load dynamic users first
  try {
    const uSaved = localStorage.getItem('pxid_users');
    DUSERS = uSaved ? JSON.parse(uSaved) : null;
  } catch(e) { DUSERS = null; }

  const restored = tryRestoreSession();
  if (restored) {
    // Valid session — go straight to app
    await loadAllData();
    document.getElementById('login-wrap').style.display = 'none';
    document.getElementById('app').style.display = 'flex';
    applyRoleUI();
    renderAll();
  } else {
    // No session — show login
    document.getElementById('login-wrap').style.display = 'flex';
    document.getElementById('app').style.display = 'none';
  }
})();
</script>
</body></html>`);
  w.document.close(); setTimeout(()=>w.print(),600);
}

// Render a daily site log report card (used in reports section)
function renderDailyLogCard(r) {
  if(!r) return '';
  const issueCount = (r.issues||[]).length;
  const openIssues = (r.issues||[]).filter(i=>i.status==='مفتوحة'||i.status==='جاري المعالجة').length;
  const photoCount = (r.photos||[]).length;
  return `<div class="dl-report-card">
    <div class="dl-report-header">
      <div>
        <div style="font-size:13px;font-weight:700;color:var(--accent);">${esc(r.projectCode||'')}</div>
        <div style="font-size:11px;color:var(--text3);">${esc(r.clientName||'—')}</div>
      </div>
      <div style="display:flex;flex-direction:column;align-items:flex-end;gap:4px;">
        <span style="font-size:12px;font-weight:700;color:var(--text1);">📅 ${r.date||'—'}</span>
        <span class="badge badge-done" style="font-size:10px;">${esc(r.status||'مُرسَل')}</span>
      </div>
    </div>
    <div class="dl-report-meta">
      <span class="dl-report-meta-item"><i class="ti ti-hard-hat"></i>${esc(r.engineerName||'—')}</span>
      ${r.workshop?`<span class="dl-report-meta-item"><i class="ti ti-building-warehouse"></i>${esc(r.workshop)}</span>`:''}
      <span class="dl-report-meta-item"><i class="ti ti-users"></i>${r.workersCount||0} عامل</span>
      ${photoCount?`<span class="dl-report-meta-item"><i class="ti ti-camera"></i>${photoCount} صورة</span>`:''}
      ${issueCount?`<span class="dl-report-meta-item" style="color:${openIssues?'var(--red)':'var(--text3)'};">
        <i class="ti ti-alert-triangle"></i>${openIssues} مشكلة مفتوحة / ${issueCount} إجمالي</span>`:''}
    </div>
    ${r.summary?`<div class="dl-report-body">${esc(r.summary)}</div>`:''}
    <div class="dl-report-actions">
      <button class="dl-action-btn" onclick="viewDailyReport('${r.id}')">
        <i class="ti ti-eye"></i> عرض
      </button>
      <button class="dl-action-btn" onclick="printDailyReport('${r.logId||r.id}',${r.projectId})">
        <i class="ti ti-printer"></i> طباعة
      </button>
      <button class="dl-action-btn" onclick="openFollowup(${r.projectId})">
        <i class="ti ti-folder-open"></i> فتح المشروع
      </button>
    </div>
  </div>`;
}

function viewDailyReport(repId) {
  const rep = STATE.reports.find(r=>r.id===repId); if(!rep) return;
  const proj = STATE.projects.find(p=>p.id===rep.projectId);
  if(proj) { openFollowup(proj.id); }
}

// ── Workshop finance expand state ──
let WS_EXPANDED = {}; // key: wsId → bool

function wsToggleDetail(wsId) {
  WS_EXPANDED[wsId] = !WS_EXPANDED[wsId];
  const panel = document.getElementById('wsd-'+wsId);
  const hdr   = document.getElementById('wsh-'+wsId);
  const ico   = document.getElementById('wsico-'+wsId);
  if(panel) panel.classList.toggle('open', !!WS_EXPANDED[wsId]);
  if(hdr)   hdr.classList.toggle('expanded', !!WS_EXPANDED[wsId]);
  if(ico)   ico.classList.toggle('open', !!WS_EXPANDED[wsId]);
}

function wsEditName(projId) {
  const nameEl = document.getElementById('wsn-'+projId);
  const inp    = document.getElementById('wsnInp-'+projId);
  if(!nameEl||!inp) return;
  nameEl.style.display = 'none';
  inp.style.display    = 'inline-block';
  inp.focus(); inp.select();
}

async function wsSaveName(projId) {
  const inp = document.getElementById('wsnInp-'+projId);
  if(!inp) return;
  const newName = inp.value.trim();
  if(!newName) return;
  const p = STATE.projects.find(x=>x.id===projId);
  if(!p) return;
  p.description = newName;
  p.updatedAt   = Date.now();
  await dbPut('projects', p);
  // Sync all views
  renderFinance();
  renderDashboard();
  renderProjects();
  if(typeof renderReports==='function') renderReports();
  toast('✓ تم تحديث اسم المشروع في جميع الأقسام');
}

// ═══ SETTINGS PERSISTENCE ═══════════════════════════════════════
async function loadSettings() {
  try {
    // Load app settings from IDB
    const saved = await new Promise((res,rej)=>{
      const tx  = DB.transaction('settings','readonly');
      const req = tx.objectStore('settings').get('main');
      req.onsuccess = ()=>res(req.result);
      req.onerror   = ()=>res(null);
    });
    if(saved) {
      Object.keys(SETTINGS).forEach(k=>{ if(saved[k]!==undefined) SETTINGS[k]=saved[k]; });
    }
    // Load activity log
    const logSaved = JSON.parse(localStorage.getItem('pxid_log')||'[]');
    ACTIVITY_LOG = Array.isArray(logSaved) ? logSaved.slice(-200) : [];
    // Load dynamic users
    const uSaved = localStorage.getItem('pxid_users');
    DUSERS = uSaved ? JSON.parse(uSaved) : [
      { id:1, username:'osman', password:'osman', role:'manager',  name:'Osman',   avatar:'أ', active:true },
      { id:2, username:'eng',   password:'eng',   role:'engineer', name:'المهندس', avatar:'م', active:true },
    ];
    // Sync USERS array used for login
    syncUsersArray();
  } catch(e){ console.warn('loadSettings error',e); }
}
async function saveSettings() {
  try {
    const tx = DB.transaction('settings','readwrite');
    tx.objectStore('settings').put({id:'main',...SETTINGS});
  } catch(e){ console.warn('saveSettings error',e); }
}
function saveDUsers() {
  localStorage.setItem('pxid_users', JSON.stringify(DUSERS));
  syncUsersArray();
}
function syncUsersArray() {
  if(DUSERS) {
    USERS.length = 0;
    DUSERS.filter(u=>u.active).forEach(u=>{
      // Ensure every user has a permissions object
      if(!u.permissions) u.permissions = {...(ROLE_DEFAULT_PERMS[u.role]||ROLE_DEFAULT_PERMS.viewer)};
      USERS.push(u);
    });
  }
}
function logActivity(action, details='') {
  const entry = { id:Date.now(), user:CU?.name||'?', action, details, time:new Date().toLocaleString('ar-SA') };
  ACTIVITY_LOG.unshift(entry);
  if(ACTIVITY_LOG.length > 200) ACTIVITY_LOG.length = 200;
  try { localStorage.setItem('pxid_log', JSON.stringify(ACTIVITY_LOG)); } catch(e){}
}

// ═══ SETTINGS TABS ═══════════════════════════════════════════════
function setTab(tab) {
  SET_TAB = tab;
  document.querySelectorAll('.set-nav-item').forEach(n=>n.classList.remove('on'));
  document.getElementById('snav-'+tab)?.classList.add('on');
  renderSetContent();
}
function renderSettings() {
  if(CU?.role==='engineer') return;
  renderSetContent();
}
function renderSetContent() {
  const el = document.getElementById('set-content');
  if(!el) return;
  switch(SET_TAB) {
    case 'company':  el.innerHTML = renderSetCompany();  break;
    case 'users':    el.innerHTML = renderSetUsers();    break;
    case 'finance':  el.innerHTML = renderSetFinance();  break;
    case 'reports':  el.innerHTML = renderSetReports();  break;
    case 'projects': el.innerHTML = renderSetProjects(); break;
    case 'security': el.innerHTML = renderSetSecurity(); break;
    case 'data':     el.innerHTML = renderSetData();     break;
    case 'log':      el.innerHTML = renderSetLog();      break;
  }
}

// ── Company Settings ──────────────────────────────────────────────
function renderSetCompany() {
  const c = SETTINGS.company;
  return `<div class="set-section">
    <div class="set-section-title"><i class="ti ti-building"></i>إعدادات الشركة / المكتب</div>
    <div class="frow"><div class="fg"><label>اسم الشركة / المكتب</label>
      <input class="fi" id="sc-name" value="${esc(c.name||'')}"></div>
      <div class="fg"><label>رقم الهاتف</label>
      <input class="fi" id="sc-phone" value="${esc(c.phone||'')}"></div></div>
    <div class="frow"><div class="fg"><label>البريد الإلكتروني</label>
      <input class="fi" id="sc-email" value="${esc(c.email||'')}"></div>
      <div class="fg"><label>الموقع الإلكتروني</label>
      <input class="fi" id="sc-web" value="${esc(c.website||'')}"></div></div>
    <div class="fg"><label>العنوان</label>
      <input class="fi" id="sc-addr" value="${esc(c.address||'')}"></div>
    <div class="frow"><div class="fg"><label>المدينة</label>
      <input class="fi" id="sc-city" value="${esc(c.city||'')}"></div>
      <div class="fg"><label>الدولة</label>
      <input class="fi" id="sc-country" value="${esc(c.country||'سوريا')}"></div></div>
    <div class="fg" style="margin-top:8px;"><label>شعار الشركة (للطباعة)</label>
      <div style="display:flex;gap:10px;align-items:center;">
        ${c.logo?`<img src="${c.logo}" style="height:50px;border-radius:6px;border:1px solid var(--border);">`:'<div style="font-size:12px;color:var(--text3);">لا يوجد شعار</div>'}
        <label class="tbtn" style="cursor:pointer;"><i class="ti ti-upload"></i> رفع شعار
          <input type="file" accept="image/*" style="display:none;" onchange="uploadCompanyLogo(this)">
        </label>
        ${c.logo?`<button class="btn-cancel" onclick="SETTINGS.company.logo=null;saveSettings();renderSetContent();">حذف</button>`:''}
      </div>
    </div>
    <div style="margin-top:14px;display:flex;gap:8px;">
      <button class="btn-save" onclick="saveCompanySettings()"><i class="ti ti-device-floppy"></i> حفظ الإعدادات</button>
    </div>
  </div>`;
}
async function saveCompanySettings() {
  SETTINGS.company = {
    ...SETTINGS.company,
    name:    document.getElementById('sc-name')?.value.trim()||'',
    phone:   document.getElementById('sc-phone')?.value.trim()||'',
    email:   document.getElementById('sc-email')?.value.trim()||'',
    website: document.getElementById('sc-web')?.value.trim()||'',
    address: document.getElementById('sc-addr')?.value.trim()||'',
    city:    document.getElementById('sc-city')?.value.trim()||'',
    country: document.getElementById('sc-country')?.value.trim()||'سوريا',
  };
  await saveSettings();
  logActivity('تعديل بيانات الشركة');
  toast('✓ تم حفظ بيانات الشركة');
  renderSetContent();
}
function uploadCompanyLogo(inp) {
  const file=inp.files[0]; if(!file) return;
  const r=new FileReader();
  r.onload=async e=>{ SETTINGS.company.logo=e.target.result; await saveSettings(); renderSetContent(); toast('✓ تم رفع الشعار'); };
  r.readAsDataURL(file); inp.value='';
}

// ── Users Management ──────────────────────────────────────────────
function renderSetUsers() {
  const roles = { manager:'مدير', engineer:'مهندس', accountant:'محاسب', viewer:'قراءة فقط' };
  const roleColors = { manager:'var(--accent)', engineer:'var(--green)', accountant:'var(--amber)', viewer:'var(--text3)' };
  const users = DUSERS || [];
  const userCards = users.map(u=>`
    <div class="user-card">
      <div class="user-avatar ${u.active?'':'inactive'}">${esc(u.avatar||u.name.charAt(0))}</div>
      <div style="flex:1;">
        <div style="font-size:13px;font-weight:700;">${esc(u.name)}</div>
        <div style="font-size:11px;color:var(--text3);">@${esc(u.username)} • <span class="user-role-badge" style="background:${roleColors[u.role]||'var(--accent-light)'}20;color:${roleColors[u.role]||'var(--accent)'};">${roles[u.role]||u.role}</span>${u.active?'':' • <span style="color:var(--red);font-size:10px;">معطّل</span>'}</div>
      </div>
      <div style="display:flex;gap:6px;">
        <button class="icon-btn edit" onclick="openEditUser(${u.id})" title="تعديل"><i class="ti ti-edit"></i> تعديل</button>
        <button class="icon-btn" onclick="toggleUser(${u.id})" title="${u.active?'تعطيل':'تفعيل'}" style="color:${u.active?'var(--amber)':'var(--green)'};">
          <i class="ti ti-${u.active?'eye-off':'eye'}"></i> ${u.active?'تعطيل':'تفعيل'}</button>
        ${u.username!=='osman'?`<button class="icon-btn del" onclick="deleteUser(${u.id})" title="حذف"><i class="ti ti-trash"></i> حذف</button>`:''}
      </div>
    </div>`).join('');
  return `<div class="set-section">
    <div class="set-section-title"><i class="ti ti-users-group"></i>إدارة المستخدمين والصلاحيات
      <button class="btn-save" style="margin-right:auto;font-size:12px;padding:6px 14px;" onclick="openAddUser()">
        <i class="ti ti-plus"></i> إضافة مستخدم
      </button>
    </div>
    ${userCards || '<div style="color:var(--text3);padding:10px 0;">لا يوجد مستخدمون</div>'}
  </div>
  <div class="set-section">
    <div class="set-section-title"><i class="ti ti-shield"></i>الصلاحيات الافتراضية لكل دور
      <span style="font-size:11px;font-weight:400;color:var(--text3);margin-right:auto;">
        تُطبَّق عند اختيار الدور — يمكن تخصيصها لكل مستخدم
      </span>
    </div>
    <div style="overflow-x:auto;">
    <table style="width:100%;border-collapse:collapse;font-size:12px;min-width:550px;">
      <thead><tr style="background:var(--surface2);">
        <th style="padding:8px 12px;text-align:right;border:1px solid var(--border);">الصلاحية</th>
        <th style="padding:8px;text-align:center;border:1px solid var(--border);">مدير</th>
        <th style="padding:8px;text-align:center;border:1px solid var(--border);">مهندس</th>
        <th style="padding:8px;text-align:center;border:1px solid var(--border);">محاسب</th>
        <th style="padding:8px;text-align:center;border:1px solid var(--border);">قراءة فقط</th>
      </tr></thead>
      <tbody>${ALL_PERMS.map(p=>`<tr>
        <td style="padding:7px 12px;border:1px solid var(--border);">${p.ar}
          <span style="font-size:9px;color:var(--text3);background:var(--surface2);padding:1px 5px;border-radius:8px;margin-right:5px;">${p.group}</span>
        </td>
        ${['manager','engineer','accountant','viewer'].map(role=>`
          <td style="padding:7px;text-align:center;border:1px solid var(--border);font-size:15px;">
            ${ROLE_DEFAULT_PERMS[role]?.[p.key]?'✅':'—'}
          </td>`).join('')}
      </tr>`).join('')}
      </tbody>
    </table>
    </div>
    <div style="margin-top:10px;font-size:12px;color:var(--text3);">
      <i class="ti ti-info-circle" style="vertical-align:-2px;"></i>
      لتعديل صلاحيات مستخدم بعينه: اضغط زر ✏️ تعديل بجانب اسمه أعلاه
    </div>
  </div>`;
}
function openAddUser() {
  const defaultRole = 'engineer';
  const permGrid = buildPermGrid(null, defaultRole);
  const panel = `<div class="set-section" id="add-user-panel">
    <div class="set-section-title"><i class="ti ti-user-plus"></i>إضافة مستخدم جديد</div>
    <div class="frow">
      <div class="fg"><label>الاسم الكامل <span class="req">*</span></label>
        <input class="fi" id="nu-name" placeholder="..."></div>
      <div class="fg"><label>اسم المستخدم <span class="req">*</span></label>
        <input class="fi" id="nu-user" placeholder="بدون مسافات"></div>
    </div>
    <div class="frow">
      <div class="fg"><label>كلمة المرور <span class="req">*</span></label>
        <input class="fi" type="password" id="nu-pass" placeholder="..."></div>
      <div class="fg"><label>الدور الأساسي</label>
        <select class="fi" id="nu-role" onchange="onRoleChange(this)">
          <option value="manager">مدير</option>
          <option value="engineer" selected>مهندس</option>
          <option value="accountant">محاسب</option>
          <option value="viewer">قراءة فقط</option>
        </select>
        <div style="font-size:10.5px;color:var(--text3);margin-top:3px;">
          تغيير الدور يُحدّث الصلاحيات تلقائياً — يمكنك تعديلها يدوياً أدناه
        </div>
      </div>
    </div>
    <div style="margin:14px 0 6px;font-size:12px;font-weight:700;color:var(--text2);">
      <i class="ti ti-shield-check" style="vertical-align:-2px;margin-left:5px;color:var(--accent);"></i>
      الصلاحيات — يمكنك تخصيصها بشكل مستقل
    </div>
    <div style="background:var(--surface2);border:1px solid var(--border);border-radius:var(--radius-sm);padding:14px;">
      ${permGrid}
    </div>
    <div style="display:flex;gap:8px;margin-top:14px;">
      <button class="btn-save" onclick="saveNewUser()"><i class="ti ti-check"></i> إضافة المستخدم</button>
      <button class="tbtn" onclick="renderSetContent()"><i class="ti ti-arrow-right"></i> رجوع</button>
      <button class="btn-cancel" onclick="renderSetContent()">إلغاء</button>
    </div>
  </div>`;
  document.getElementById('set-content').insertAdjacentHTML('afterbegin', panel);
}
function saveNewUser() {
  const name = document.getElementById('nu-name')?.value.trim();
  const uname= document.getElementById('nu-user')?.value.trim().toLowerCase();
  const pass = document.getElementById('nu-pass')?.value;
  const role = document.getElementById('nu-role')?.value||'engineer';
  if(!name||!uname||!pass){ toast('⚠ أدخل جميع الحقول المطلوبة'); return; }
  if((DUSERS||[]).find(u=>u.username===uname)){ toast('⚠ اسم المستخدم موجود مسبقاً'); return; }
  const permissions = readPermGrid();
  const newUser = { id:Date.now(), username:uname, password:pass, role, name, avatar:name.charAt(0), active:true, permissions };
  (DUSERS||[]).push(newUser);
  saveDUsers();
  logActivity(`إضافة مستخدم: ${name}`);
  toast('✓ تم إضافة المستخدم');
  renderSetContent();
}
function openEditUser(uid) {
  const u = (DUSERS||[]).find(x=>x.id===uid); if(!u) return;
  if(!u.permissions) u.permissions = {...(ROLE_DEFAULT_PERMS[u.role]||{})};
  const permGrid = buildPermGrid(u.permissions, u.role);
  const panel = `<div class="set-section" id="edit-user-panel">
    <div class="set-section-title"><i class="ti ti-user-edit"></i>تعديل: ${esc(u.name)}</div>
    <div class="frow">
      <div class="fg"><label>الاسم الكامل</label>
        <input class="fi" id="eu-name" value="${esc(u.name)}"></div>
      <div class="fg"><label>الدور الأساسي</label>
        <select class="fi" id="eu-role" onchange="onRoleChange(this)">
          <option value="manager"    ${u.role==='manager'   ?'selected':''}>مدير</option>
          <option value="engineer"   ${u.role==='engineer'  ?'selected':''}>مهندس</option>
          <option value="accountant" ${u.role==='accountant'?'selected':''}>محاسب</option>
          <option value="viewer"     ${u.role==='viewer'    ?'selected':''}>قراءة فقط</option>
        </select>
        <div style="font-size:10.5px;color:var(--text3);margin-top:3px;">
          تغيير الدور يُعيد ضبط الصلاحيات للقيم الافتراضية
        </div>
      </div>
    </div>
    <div class="fg"><label>كلمة مرور جديدة <span style="color:var(--text3);font-weight:400;">(اتركه فارغاً لعدم التغيير)</span></label>
      <input class="fi" type="password" id="eu-pass" placeholder="(اختياري)"></div>
    <div style="margin:14px 0 6px;font-size:12px;font-weight:700;color:var(--text2);">
      <i class="ti ti-shield-check" style="vertical-align:-2px;margin-left:5px;color:var(--accent);"></i>
      الصلاحيات المخصصة
    </div>
    <div style="background:var(--surface2);border:1px solid var(--border);border-radius:var(--radius-sm);padding:14px;">
      ${permGrid}
    </div>
    <div style="display:flex;gap:8px;margin-top:14px;">
      <button class="btn-save" onclick="saveEditUser(${uid})"><i class="ti ti-check"></i> حفظ التغييرات</button>
      <button class="btn-cancel" onclick="renderSetContent()">إلغاء</button>
    </div>
  </div>`;
  document.getElementById('set-content').insertAdjacentHTML('afterbegin', panel);
}
function saveEditUser(uid) {
  const u = (DUSERS||[]).find(x=>x.id===uid); if(!u) return;
  u.name = document.getElementById('eu-name')?.value.trim()||u.name;
  u.role = document.getElementById('eu-role')?.value||u.role;
  u.avatar = u.name.charAt(0);
  const newPass = document.getElementById('eu-pass')?.value;
  if(newPass) u.password = newPass;
  // Save custom permissions from checkboxes
  u.permissions = readPermGrid();
  // If this is the currently logged-in user, update CU.permissions live
  if(CU && CU.username === u.username) {
    CU.permissions = {...u.permissions};
    try { localStorage.setItem('pxid_session', JSON.stringify(CU)); } catch(e){}
    applyRoleUI();
  }
  saveDUsers();
  logActivity(`تعديل مستخدم: ${u.name}`);
  toast('✓ تم تعديل المستخدم');
  renderSetContent();
}
function toggleUser(uid) {
  const u = (DUSERS||[]).find(x=>x.id===uid); if(!u) return;
  if(u.username==='osman'){ toast('⚠ لا يمكن تعطيل حساب المدير الرئيسي'); return; }
  u.active = !u.active;
  saveDUsers();
  logActivity(`${u.active?'تفعيل':'تعطيل'} مستخدم: ${u.name}`);
  toast(u.active?'✓ تم تفعيل الحساب':'⚠ تم تعطيل الحساب');
  renderSetContent();
}
function deleteUser(uid) {
  const u = (DUSERS||[]).find(x=>x.id===uid); if(!u) return;
  if(u.username==='osman'){ toast('⚠ لا يمكن حذف حساب المدير الرئيسي'); return; }
  if(!confirm(`حذف المستخدم "${u.name}"؟`)) return;
  DUSERS.splice(DUSERS.indexOf(u),1);
  saveDUsers();
  logActivity(`حذف مستخدم: ${u.name}`);
  toast('تم حذف المستخدم');
  renderSetContent();
}

// ── Finance Settings ──────────────────────────────────────────────
function renderSetFinance() {
  const f = SETTINGS.finance;
  const methods = f.paymentMethods || [];
  return `<div class="set-section">
    <div class="set-section-title"><i class="ti ti-coin"></i>إعدادات الشؤون المالية</div>
    <div class="fg"><label>العملة الافتراضية</label>
      <select class="fi" id="sf-cur" style="width:200px;">
        ${['USD','SYP','EUR','SAR','AED','TRY'].map(c=>`<option ${f.defaultCurrency===c?'selected':''}>${c}</option>`).join('')}
      </select>
    </div>
    <div class="fg" style="margin-top:12px;">
      <label>طرق الدفع المتاحة</label>
      <div class="tag-list" id="sf-methods-list">
        ${methods.map((m,i)=>`<span class="tag-item">${esc(m)}<button class="tag-del" onclick="sfRemoveMethod(${i})" title="حذف"> ✕ حذف</button></span>`).join('')}
      </div>
      <div class="tag-add-row">
        <input class="fi" id="sf-method-inp" placeholder="أضف طريقة دفع..." style="flex:1;">
        <button class="tbtn" onclick="sfAddMethod()"><i class="ti ti-plus"></i> إضافة</button>
      </div>
    </div>
    <div class="set-toggle-row" style="margin-top:12px;">
      <div><div class="set-toggle-lbl">ضريبة القيمة المضافة (VAT)</div>
        <div class="set-toggle-sub">تطبيق ضريبة على الفواتير</div>
      </div>
      <label class="toggle-sw"><input type="checkbox" id="sf-vat" ${f.vatEnabled?'checked':''}
        onchange="SETTINGS.finance.vatEnabled=this.checked;">
        <span class="toggle-track"></span></label>
    </div>
    <div class="fg" style="margin-top:8px;">
      <label>نسبة الضريبة %</label>
      <input class="fi" type="number" id="sf-vat-rate" value="${f.vatRate||0}" min="0" max="100" style="width:100px;">
    </div>
    <div style="margin-top:14px;">
      <button class="btn-save" onclick="saveFinanceSettings()"><i class="ti ti-device-floppy"></i> حفظ</button>
    </div>
  </div>`;
}
function sfAddMethod() {
  const inp=document.getElementById('sf-method-inp');
  const val=inp.value.trim(); if(!val) return;
  if(!SETTINGS.finance.paymentMethods) SETTINGS.finance.paymentMethods=[];
  SETTINGS.finance.paymentMethods.push(val);
  inp.value='';
  renderSetContent();
}
function sfRemoveMethod(i) {
  SETTINGS.finance.paymentMethods.splice(i,1);
  renderSetContent();
}
async function saveFinanceSettings() {
  SETTINGS.finance.defaultCurrency = document.getElementById('sf-cur')?.value||'USD';
  SETTINGS.finance.vatRate = parseFloat(document.getElementById('sf-vat-rate')?.value)||0;
  await saveSettings();
  logActivity('تعديل إعدادات الشؤون المالية');
  toast('✓ تم حفظ إعدادات المالية');
}

// ── Reports Settings ──────────────────────────────────────────────
function renderSetReports() {
  const r = SETTINGS.reports;
  const toggles = [
    ['showLogo','شعار الشركة في الطباعة','يظهر الشعار في رأس التقارير المطبوعة'],
    ['showClient','بيانات العميل','اسم ومعلومات العميل في التقرير'],
    ['showEngineer','اسم المهندس','اسم المهندس المسؤول'],
    ['showPhotos','الصور والمرفقات','تضمين الصور في التقرير'],
    ['showSignature','حقل التوقيع','مساحة للتوقيع في نهاية التقرير'],
    ['showNotes','الملاحظات','إظهار حقل الملاحظات'],
  ];
  return `<div class="set-section">
    <div class="set-section-title"><i class="ti ti-report"></i>إعدادات التقارير</div>
    <div class="frow"><div class="fg"><label>بادئة ترقيم التقارير</label>
      <input class="fi" id="sr-prefix" value="${esc(r.prefix||'REP')}" style="width:130px;">
      <div style="font-size:11px;color:var(--text3);margin-top:3px;">مثال: ${esc(r.prefix||'REP')}-2026-001</div>
    </div></div>
    <div style="margin-top:14px;">
      <div style="font-size:12px;font-weight:700;color:var(--text2);margin-bottom:8px;">خيارات الطباعة</div>
      ${toggles.map(([key,lbl,sub])=>`
        <div class="set-toggle-row">
          <div><div class="set-toggle-lbl">${lbl}</div><div class="set-toggle-sub">${sub}</div></div>
          <label class="toggle-sw"><input type="checkbox" ${r[key]?'checked':''}
            onchange="SETTINGS.reports['${key}']=this.checked;saveSettings();">
            <span class="toggle-track"></span></label>
        </div>`).join('')}
    </div>
    <div style="margin-top:14px;">
      <button class="btn-save" onclick="saveReportsSettings()"><i class="ti ti-device-floppy"></i> حفظ</button>
    </div>
  </div>`;
}
async function saveReportsSettings() {
  SETTINGS.reports.prefix = document.getElementById('sr-prefix')?.value.trim()||'REP';
  await saveSettings();
  logActivity('تعديل إعدادات التقارير');
  toast('✓ تم حفظ إعدادات التقارير');
}

// ── Projects Settings ─────────────────────────────────────────────
function renderSetProjects() {
  const ws = SETTINGS.workshopTypes||[];
  const wk = SETTINGS.workerTypes||[];
  return `<div class="set-section">
    <div class="set-section-title"><i class="ti ti-building-warehouse"></i>أنواع الورشات</div>
    <div class="tag-list" id="sp-ws-list">
      ${ws.map((w,i)=>`<span class="tag-item">${esc(w)}<button class="tag-del" onclick="spRemoveWs(${i})" title="حذف"> ✕ حذف</button></span>`).join('')}
    </div>
    <div style="font-size:11px;color:var(--green);margin:4px 0;"><i class="ti ti-info-circle" style="vertical-align:-2px;"></i> تظهر الأنواع المضافة هنا تلقائياً في قسم المتابعة</div>
    <div class="tag-add-row">
      <input class="fi" id="sp-ws-inp" placeholder="نوع ورشة جديد..." onkeydown="if(event.key==='Enter')spAddWs()">
      <button class="tbtn" onclick="spAddWs()"><i class="ti ti-plus"></i> إضافة</button>
    </div>
  </div>
  <div class="set-section">
    <div class="set-section-title"><i class="ti ti-hard-hat"></i>أنواع العمال</div>
    <div class="tag-list">
      ${wk.map((w,i)=>`<span class="tag-item">${esc(w)}<button class="tag-del" onclick="spRemoveWk(${i})" title="حذف"> ✕ حذف</button></span>`).join('')}
    </div>
    <div class="tag-add-row">
      <input class="fi" id="sp-wk-inp" placeholder="نوع عامل جديد...">
      <button class="tbtn" onclick="spAddWk()"><i class="ti ti-plus"></i> إضافة</button>
    </div>
  </div>`;
}
async function spAddWs(){
  const v=document.getElementById('sp-ws-inp')?.value.trim();
  if(!v){toast('⚠ أدخل اسم نوع الورشة');return;}
  if(!SETTINGS.workshopTypes) SETTINGS.workshopTypes=[];
  if(SETTINGS.workshopTypes.includes(v)){toast('⚠ هذا النوع موجود مسبقاً');return;}
  SETTINGS.workshopTypes.unshift(v); // add to top
  document.getElementById('sp-ws-inp').value='';
  await saveSettings();
  renderSetContent();
  // Sync followup if open
  if(FU_CUR && document.getElementById('followup-overlay')?.classList.contains('open')) fuRender();
  toast('✓ تم إضافة نوع الورشة — يظهر الآن في قسم المتابعة');
}
async function spRemoveWs(i){SETTINGS.workshopTypes.splice(i,1);await saveSettings();renderSetContent();}
async function spAddWk(){const v=document.getElementById('sp-wk-inp')?.value.trim();if(!v)return;SETTINGS.workerTypes.push(v);document.getElementById('sp-wk-inp').value='';await saveSettings();renderSetContent();}
async function spRemoveWk(i){SETTINGS.workerTypes.splice(i,1);await saveSettings();renderSetContent();}

// ── Security Settings ─────────────────────────────────────────────
function renderSetSecurity() {
  return `<div class="set-section">
    <div class="set-section-title"><i class="ti ti-lock"></i>تغيير كلمة المرور</div>
    <div class="fg"><label>كلمة المرور الحالية</label>
      <input class="fi" type="password" id="sec-old" placeholder="..."></div>
    <div class="fg" style="margin-top:8px;"><label>كلمة المرور الجديدة</label>
      <input class="fi" type="password" id="sec-new" placeholder="..."></div>
    <div class="fg" style="margin-top:8px;"><label>تأكيد كلمة المرور الجديدة</label>
      <input class="fi" type="password" id="sec-confirm" placeholder="..."></div>
    <div style="margin-top:14px;">
      <button class="btn-save" onclick="changePassword()"><i class="ti ti-key"></i> تغيير كلمة المرور</button>
    </div>
  </div>
  <div class="set-section">
    <div class="set-section-title"><i class="ti ti-clock"></i>مهلة الجلسة</div>
    <div class="fg"><label>تسجيل الخروج التلقائي بعد (دقيقة) — 0 = لا يوجد</label>
      <input class="fi" type="number" id="sec-timeout" min="0" value="${SETTINGS.sessionTimeout||0}" style="width:100px;">
    </div>
    <div style="margin-top:10px;">
      <button class="btn-save" onclick="saveSecSettings()"><i class="ti ti-device-floppy"></i> حفظ</button>
    </div>
  </div>`;
}
async function changePassword() {
  const oldP=document.getElementById('sec-old')?.value;
  const newP=document.getElementById('sec-new')?.value;
  const conf=document.getElementById('sec-confirm')?.value;
  const u = (DUSERS||[]).find(x=>x.username===CU.username);
  if(!u){ toast('⚠ خطأ في تحديد المستخدم'); return; }
  if(u.password!==oldP){ toast('⚠ كلمة المرور الحالية غير صحيحة'); return; }
  if(!newP||newP.length<3){ toast('⚠ كلمة المرور يجب أن تكون 3 أحرف على الأقل'); return; }
  if(newP!==conf){ toast('⚠ كلمة المرور الجديدة غير متطابقة'); return; }
  u.password=newP;
  saveDUsers();
  logActivity('تغيير كلمة المرور');
  toast('✓ تم تغيير كلمة المرور');
  ['sec-old','sec-new','sec-confirm'].forEach(id=>{ const el=document.getElementById(id); if(el) el.value=''; });
}
async function saveSecSettings() {
  SETTINGS.sessionTimeout = parseInt(document.getElementById('sec-timeout')?.value)||0;
  await saveSettings();
  toast('✓ تم حفظ إعدادات الأمان');
}

// ── Data Management ───────────────────────────────────────────────
function renderSetData() {
  const projCount = STATE.projects.length;
  const clientCount = STATE.clients.length;
  const repCount = STATE.reports.length;
  return `<div class="set-section">
    <div class="set-section-title"><i class="ti ti-database-export"></i>تصدير البيانات</div>
    <div style="display:grid;grid-template-columns:repeat(3,1fr);gap:10px;margin-bottom:14px;">
      <div style="background:var(--surface2);border-radius:var(--radius-sm);padding:12px;text-align:center;">
        <div style="font-size:22px;font-weight:700;">${projCount}</div>
        <div style="font-size:11px;color:var(--text3);">مشروع</div>
      </div>
      <div style="background:var(--surface2);border-radius:var(--radius-sm);padding:12px;text-align:center;">
        <div style="font-size:22px;font-weight:700;">${clientCount}</div>
        <div style="font-size:11px;color:var(--text3);">عميل</div>
      </div>
      <div style="background:var(--surface2);border-radius:var(--radius-sm);padding:12px;text-align:center;">
        <div style="font-size:22px;font-weight:700;">${repCount}</div>
        <div style="font-size:11px;color:var(--text3);">تقرير</div>
      </div>
    </div>
    <div style="display:flex;gap:8px;flex-wrap:wrap;">
      <button class="tbtn" onclick="exportData()"><i class="ti ti-download"></i> تصدير كامل (JSON)</button>
      <button class="tbtn" onclick="exportProjectsCsv()"><i class="ti ti-file-spreadsheet"></i> تصدير المشاريع (CSV)</button>
    </div>
  </div>
  <div class="set-section">
    <div class="set-section-title"><i class="ti ti-database-import"></i>استيراد البيانات</div>
    <div class="fg"><label>استيراد ملف JSON (تصدير سابق)</label>
      <label class="tbtn" style="cursor:pointer;"><i class="ti ti-upload"></i> اختر ملف JSON
        <input type="file" accept=".json" style="display:none;" onchange="importData(this)">
      </label>
    </div>
  </div>
  <div class="set-section" style="border-color:var(--red);">
    <div class="set-section-title" style="color:var(--red);"><i class="ti ti-alert-triangle"></i>منطقة الخطر</div>
    <div style="font-size:12px;color:var(--text3);margin-bottom:10px;">هذه الإجراءات لا يمكن التراجع عنها.</div>
    <div style="display:flex;gap:8px;flex-wrap:wrap;">
      <button class="tbtn" style="color:var(--red);border-color:var(--red);"
        onclick="if(confirm('حذف جميع البيانات؟ هذا الإجراء لا يمكن التراجع عنه!')){clearAll();}">
        <i class="ti ti-trash"></i> مسح جميع البيانات
      </button>
      <button class="tbtn" style="color:var(--amber);border-color:var(--amber);"
        onclick="if(confirm('مسح سجل النشاط؟')){ACTIVITY_LOG=[];localStorage.removeItem(\'pxid_log\');toast(\'تم مسح السجل\');}">
        <i class="ti ti-history"></i> مسح سجل النشاط
      </button>
    </div>
  </div>`;
}
function exportProjectsCsv() {
  const rows = STATE.projects.map(p=>{
    const c = STATE.clients.find(cl=>cl.id===p.clientId);
    const t = TYPES[p.taskTypeKey]||{};
    return [p.projectCode, t.ar||'', c?.name||'', p.description||'', p.status||'', p.deliveryDate||''];
  });
  const csvHeader = ['Project','Type','Client','Description','Status','Delivery Date'].join(',');
  const csv = csvHeader + '\n' + rows.map(r=>r.map(v=>'"'+String(v||'').replace(/"/g,"'")+'"').join(',')).join('\n');
  const a=document.createElement('a');
  a.href=URL.createObjectURL(new Blob(['﻿'+csv],{type:'text/csv;charset=utf-8'}));
  a.download='projects_'+new Date().toISOString().split('T')[0]+'.csv';
  a.click();
}
async function importData(inp) {
  const file=inp.files[0]; if(!file) return;
  const text=await file.text();
  try {
    const data=JSON.parse(text);
    if(!confirm(`استيراد: ${(data.projects||[]).length} مشروع، ${(data.clients||[]).length} عميل؟`)) return;
    if(data.clients)  { STATE.clients  = data.clients;  for(const c of STATE.clients)  await dbPut('clients',c); }
    if(data.projects) { STATE.projects = data.projects; for(const p of STATE.projects) await dbPut('projects',p); }
    if(data.engineers){ STATE.engineers= data.engineers;for(const e of STATE.engineers)await dbPut('engineers',e); }
    if(data.reports)  { STATE.reports  = data.reports;  for(const r of STATE.reports)  await dbPut('reports',r); }
    logActivity('استيراد بيانات من ملف');
    toast('✓ تم الاستيراد بنجاح');
    renderAll();
  } catch(e){ toast('⚠ ملف غير صالح'); }
  inp.value='';
}

// ── Activity Log ──────────────────────────────────────────────────
function renderSetLog() {
  const logs = ACTIVITY_LOG.slice(0,100);
  if(!logs.length) return `<div class="set-section"><div class="empty"><i class="ti ti-history"></i><p>لا يوجد نشاط مسجّل بعد</p></div></div>`;
  return `<div class="set-section">
    <div class="set-section-title"><i class="ti ti-history"></i>سجل النشاط (آخر 100 عملية)
      <span style="font-size:11px;font-weight:400;color:var(--text3);margin-right:auto;">${logs.length} عملية مسجّلة</span>
    </div>
    ${logs.map(l=>`<div class="log-row">
      <div class="log-dot"></div>
      <div style="flex:1;">
        <span class="log-user">${esc(l.user)}</span>
        <span style="color:var(--text2);"> — ${esc(l.action)}</span>
        ${l.details?`<span style="font-size:11px;color:var(--text3);"> (${esc(l.details)})</span>`:''}
      </div>
      <span class="log-time">${l.time}</span>
    </div>`).join('')}
  </div>`;
}

// Build interactive permissions grid
function buildPermGrid(existingPerms, roleDefault) {
  const groups = {};
  ALL_PERMS.forEach(p => {
    if(!groups[p.group]) groups[p.group] = [];
    groups[p.group].push(p);
  });
  const checked = existingPerms || {...(ROLE_DEFAULT_PERMS[roleDefault]||{})};
  return Object.entries(groups).map(([grp, perms])=>`
    <div style="margin-bottom:12px;">
      <div style="font-size:11px;font-weight:700;color:var(--text3);text-transform:uppercase;
        letter-spacing:.5px;margin-bottom:6px;padding-bottom:4px;border-bottom:1px solid var(--border);">
        ${grp}
      </div>
      <div style="display:grid;grid-template-columns:1fr 1fr;gap:4px;">
        ${perms.map(p=>`
          <label style="display:flex;align-items:center;gap:7px;padding:5px 8px;
            border-radius:6px;cursor:pointer;border:1px solid var(--border);
            background:${checked[p.key]?'var(--accent-light)':'var(--surface)'};
            transition:background .12s;" class="perm-cb-wrap">
            <input type="checkbox" class="perm-cb" data-key="${p.key}"
              ${checked[p.key]?'checked':''}
              onchange="this.closest('label').style.background=this.checked?'var(--accent-light)':'var(--surface)';"
              style="accent-color:var(--accent);width:15px;height:15px;">
            <span style="font-size:12px;color:var(--text1);">${p.ar}</span>
          </label>`).join('')}
      </div>
    </div>`).join('');
}

// Read permissions from rendered checkboxes
function readPermGrid() {
  const result = {};
  document.querySelectorAll('.perm-cb').forEach(cb=>{
    result[cb.dataset.key] = cb.checked ? 1 : 0;
  });
  return result;
}

// When role changes in the form — update checkboxes to role defaults
function onRoleChange(selectEl) {
  const role = selectEl.value;
  const defaults = ROLE_DEFAULT_PERMS[role]||{};
  document.querySelectorAll('.perm-cb').forEach(cb=>{
    cb.checked = !!defaults[cb.dataset.key];
    cb.closest('label').style.background = cb.checked?'var(--accent-light)':'var(--surface)';
  });
}

// Workshop Financial Summary Print
function printWorkshopSummary() {
  const projects = STATE.projects.filter(p=>isExecType(p));
  if(!projects.length) { toast('⚠ لا توجد مشاريع تنفيذية'); return; }

  let totalWsContract=0, totalWsPaid=0, totalWkCost=0, totalWkPaid=0;
  let rows = '';
  let wsDetailRows = '';

  projects.forEach(p=>{
    const c   = STATE.clients.find(cl=>cl.id===p.clientId);
    const fin = getProjFin(p);
    const cur = fin.currency || p.currency || 'USD';
    const wft = calcWorkforceTotals(p);
    totalWsContract += wft.wsContract;
    totalWsPaid     += wft.wsPaid;
    totalWkCost     += wft.wkCost;
    totalWkPaid     += wft.wkPaidAmt;

    // Project summary row
    rows += `<tr style="border-bottom:1px solid #e5e7eb;">
      <td style="padding:8px 12px;font-weight:700;color:#534AB7;font-family:monospace;">${esc(p.projectCode)}</td>
      <td style="padding:8px 12px;">${esc(c?.name||'—')}</td>
      <td style="padding:8px 12px;">${(p.workforce?.workshops||[]).length} ورشة</td>
      <td style="padding:8px 12px;">${fmt(wft.wsContract,cur)}</td>
      <td style="padding:8px 12px;color:#16a34a;">${fmt(wft.wsPaid,cur)}</td>
      <td style="padding:8px 12px;color:${wft.wsRem>0?'#dc2626':'#16a34a'};">${wft.wsRem>0?fmt(wft.wsRem,cur):'✓ مسدد'}</td>
      <td style="padding:8px 12px;color:#d97706;">${fmt(wft.wkCost,cur)}</td>
      <td style="padding:8px 12px;color:#16a34a;">${fmt(wft.wkPaidAmt,cur)}</td>
    </tr>`;

    // Workshop detail rows
    (p.workforce?.workshops||[]).forEach(ws=>{
      const total = spTotal(ws), paid = spPaid(ws), rem = total-paid;
      const pct   = total ? Math.round(paid/total*100) : 0;
      wsDetailRows += `<tr style="border-bottom:1px solid #f0f0f0;">
        <td style="padding:6px 10px;color:#888;font-size:11px;">${esc(p.projectCode)}</td>
        <td style="padding:6px 10px;font-weight:600;">${esc(ws.name||'—')}</td>
        <td style="padding:6px 10px;color:#666;">${esc(ws.type||'—')}</td>
        <td style="padding:6px 10px;">${ws.qty||0} ${esc(ws.unit||'')} × ${fmt(ws.unitPrice||0,cur)}</td>
        <td style="padding:6px 10px;font-weight:700;">${fmt(total,cur)}</td>
        <td style="padding:6px 10px;color:#16a34a;">${fmt(paid,cur)}</td>
        <td style="padding:6px 10px;color:${rem>0?'#dc2626':'#16a34a'};">${rem>0?fmt(rem,cur):'✓'}</td>
        <td style="padding:6px 10px;">${ws.progress||0}%</td>
        <td style="padding:6px 10px;font-size:10px;color:#888;">${(ws.payments||[]).length} دفعة</td>
      </tr>`;
    });
  });

  const co   = SETTINGS?.company || {};
  const date = new Date().toLocaleDateString('ar-SA');
  const w    = window.open('','_blank','width=1000,height:1300');
  w.document.write(`<!DOCTYPE html><html dir="rtl" lang="ar"><head><meta charset="UTF-8">
    <title>الملخص المالي الشامل — الورشات والعمال</title>
    <style>
      body{font-family:'Segoe UI',Tahoma,sans-serif;padding:24px;direction:rtl;color:#1c1c1a;margin:0;}
      h1{font-size:20px;margin:0 0 4px;}
      h2{font-size:14px;color:#534AB7;border-bottom:2px solid #534AB7;padding-bottom:5px;margin:22px 0 10px;}
      table{width:100%;border-collapse:collapse;font-size:12px;}
      th{background:#534AB7;color:#fff;padding:9px 12px;text-align:right;}
      .kpi-grid{display:grid;grid-template-columns:repeat(4,1fr);gap:10px;margin:14px 0;}
      .kpi{background:#f5f5f5;border-radius:8px;padding:12px;text-align:center;}
      .kpi-lbl{font-size:9.5px;color:#999;margin-bottom:3px;}
      .kpi-val{font-size:15px;font-weight:700;}
      @media print{body{padding:14px;}button{display:none;}}
    </style>
  </head><body>
    <div style="display:flex;justify-content:space-between;align-items:flex-start;border-bottom:3px solid #534AB7;padding-bottom:12px;margin-bottom:16px;">
      <div>
        <h1>📊 الملخص المالي الشامل — الورشات والعمال</h1>
        <p style="color:#666;margin:4px 0;">${esc(co.name||'ProjexID')} • ${date}</p>
      </div>
      <button onclick="window.print()" style="padding:8px 18px;background:#534AB7;color:#fff;border:none;border-radius:6px;cursor:pointer;font-size:13px;">🖨 طباعة</button>
    </div>
    <!-- Global KPIs -->
    <div class="kpi-grid">
      <div class="kpi"><div class="kpi-lbl">إجمالي عقود الورشات</div><div class="kpi-val" style="color:#534AB7;">${fmt(totalWsContract,'USD')}</div></div>
      <div class="kpi"><div class="kpi-lbl">مدفوع للورشات</div><div class="kpi-val" style="color:#16a34a;">${fmt(totalWsPaid,'USD')}</div></div>
      <div class="kpi"><div class="kpi-lbl">متبقي للورشات</div><div class="kpi-val" style="color:#dc2626;">${fmt(totalWsContract-totalWsPaid,'USD')}</div></div>
      <div class="kpi"><div class="kpi-lbl">تكلفة العمال</div><div class="kpi-val" style="color:#d97706;">${fmt(totalWkCost,'USD')}</div></div>
    </div>
    <!-- Projects summary -->
    <h2>ملخص المشاريع التنفيذية</h2>
    <table><thead><tr>
      <th>المشروع</th><th>العميل</th><th>الورشات</th>
      <th>عقود الورشات</th><th>مدفوع</th><th>متبقي</th>
      <th>تكلفة العمال</th><th>مدفوع للعمال</th>
    </tr></thead><tbody>${rows}</tbody></table>
    <!-- Workshop details -->
    <h2>تفاصيل الورشات</h2>
    <table><thead><tr>
      <th>المشروع</th><th>الورشة</th><th>نوع العمل</th><th>الكمية × السعر</th>
      <th>قيمة العقد</th><th>مدفوع</th><th>متبقي</th><th>إنجاز</th><th>الدفعات</th>
    </tr></thead><tbody>${wsDetailRows}</tbody></table>
    <p style="margin-top:24px;font-size:10px;color:#999;border-top:1px solid #eee;padding-top:8px;">
      * الإجماليات بالدولار تقريبية للمشاريع ذات العملات المختلطة • طُبع من ProjexID — ${date}
    </p>
  
<script>
// ── Startup: check session then show login or app ──
(async function startApp() {
  await initDB();
  // Load dynamic users first
  try {
    const uSaved = localStorage.getItem('pxid_users');
    DUSERS = uSaved ? JSON.parse(uSaved) : null;
  } catch(e) { DUSERS = null; }

  const restored = tryRestoreSession();
  if (restored) {
    // Valid session — go straight to app
    await loadAllData();
    document.getElementById('login-wrap').style.display = 'none';
    document.getElementById('app').style.display = 'flex';
    applyRoleUI();
    renderAll();
  } else {
    // No session — show login
    document.getElementById('login-wrap').style.display = 'flex';
    document.getElementById('app').style.display = 'none';
  }
})();
</script>
</body></html>`);
  w.document.close();
  setTimeout(()=>w.print(),600);
}

// ── Print single project workshops ───────────────────────────────
function printProjectWorkshops(projId) {
  const p   = STATE.projects.find(x=>x.id===projId); if(!p) return;
  const c   = STATE.clients.find(cl=>cl.id===p.clientId);
  const fin = getProjFin(p);
  const cur = fin.currency || p.currency || 'USD';
  const wks = p.workforce?.workshops || [];
  const t   = TYPES[p.taskTypeKey]||{};
  const co  = SETTINGS?.company||{};
  const wft = calcWorkforceTotals(p);
  const date = new Date().toLocaleDateString('ar-SA');

  const wsRows = wks.map((ws,idx)=>{
    const total=spTotal(ws), paid=spPaid(ws), rem=total-paid;
    const pct=total?Math.round(paid/total*100):0;
    const payList=(ws.payments||[]).map((pm,i)=>`
      <tr style="background:#fafafa;">
        <td style="padding:5px 10px;color:#888;">${i+1}</td>
        <td style="padding:5px 10px;">${payTypeLabel(pm.type)}</td>
        <td style="padding:5px 10px;">${pm.date||'—'}</td>
        <td style="padding:5px 10px;color:#16a34a;font-weight:700;">${fmt(pm.amount||0,cur)}</td>
        <td style="padding:5px 10px;color:#888;">${payMethodLabel(pm.method)} ${pm.ref?'• '+esc(pm.ref):''}</td>
        <td style="padding:5px 10px;color:#888;">${esc(pm.notes||'')}</td>
      </tr>`).join('');
    return `
      <tr style="background:#ede9ff;font-weight:700;border-top:2px solid #534AB7;">
        <td colspan="7" style="padding:8px 12px;color:#534AB7;font-size:13px;">
          ${idx+1}. ${esc(ws.name||'ورشة')} — ${esc(ws.type||'')} ${ws.item?'— '+esc(ws.item):''}
        </td>
      </tr>
      <tr>
        <td style="padding:6px 12px;" colspan="2"><b>المسؤول:</b> ${esc(ws.manager||'—')} ${ws.phone?'📞 '+esc(ws.phone):''}</td>
        <td style="padding:6px 12px;"><b>الكمية:</b> ${ws.qty||0} ${esc(ws.unit||'')}</td>
        <td style="padding:6px 12px;"><b>سعر الوحدة:</b> ${fmt(ws.unitPrice||0,cur)}</td>
        <td style="padding:6px 12px;font-weight:700;color:#534AB7;"><b>قيمة العقد:</b> ${fmt(total,cur)}</td>
        <td style="padding:6px 12px;color:#16a34a;"><b>مدفوع:</b> ${fmt(paid,cur)} (${pct}%)</td>
        <td style="padding:6px 12px;color:${rem>0?'#dc2626':'#16a34a'};"><b>متبقي:</b> ${rem>0?fmt(rem,cur):'✓ مسدد'}</td>
      </tr>
      ${payList ? `
        <tr><td colspan="7" style="padding:4px 12px;font-size:11px;color:#888;background:#f9f9f9;">
          سجل الدفعات (${ws.payments.length}):
        </td></tr>
        ${payList}` : ''}`;
  }).join('');

  const w = window.open('','_blank','width=900,height:1200');
  w.document.write(`<!DOCTYPE html><html dir="rtl" lang="ar"><head><meta charset="UTF-8">
    <title>حساب الورشات — ${esc(p.projectCode)}</title>
    <style>body{font-family:'Segoe UI',Tahoma,sans-serif;padding:24px;direction:rtl;color:#1c1c1a;}
    h1{font-size:19px;margin:0;}h2{font-size:13px;color:#534AB7;border-bottom:2px solid #534AB7;padding-bottom:4px;margin:18px 0 10px;}
    table{width:100%;border-collapse:collapse;font-size:12px;}
    td,th{border:1px solid #e5e7eb;text-align:right;vertical-align:top;}
    th{background:#534AB7;color:#fff;padding:8px 12px;}
    .kpi{display:inline-block;background:#f5f5f5;border-radius:8px;padding:10px 16px;margin:4px;text-align:center;}
    .kpi-v{font-size:16px;font-weight:700;}.kpi-l{font-size:10px;color:#888;}
    @media print{body{padding:12px;}button{display:none;}}</style>
  </head><body>
    <div style="display:flex;justify-content:space-between;align-items:flex-start;border-bottom:3px solid #534AB7;padding-bottom:10px;margin-bottom:14px;">
      <div>
        <h1>🏗️ حساب الورشات — ${esc(p.projectCode)}</h1>
        <div style="color:#666;margin-top:6px;font-size:12px;">
          <b>العميل:</b> ${esc(c?.name||'—')} &nbsp;|&nbsp;
          <b>النوع:</b> ${t.icon||''} ${t.ar||''} &nbsp;|&nbsp;
          ${p.propertyNumber?`<b>رقم العقار:</b> ${esc(p.propertyNumber)} &nbsp;|&nbsp;`:''}
          ${p.district?`<b>المنطقة:</b> ${esc(p.district)} &nbsp;|&nbsp;`:''}
          <b>تاريخ الطباعة:</b> ${date}
        </div>
      </div>
      <button onclick="window.print()" style="padding:8px 16px;background:#534AB7;color:#fff;border:none;border-radius:6px;cursor:pointer;">🖨 طباعة</button>
    </div>
    <!-- KPIs -->
    <div style="margin-bottom:16px;">
      <div class="kpi"><div class="kpi-v" style="color:#534AB7;">${fmt(wft.wsContract,cur)}</div><div class="kpi-l">إجمالي عقود الورشات</div></div>
      <div class="kpi"><div class="kpi-v" style="color:#16a34a;">${fmt(wft.wsPaid,cur)}</div><div class="kpi-l">المدفوع</div></div>
      <div class="kpi"><div class="kpi-v" style="color:${wft.wsRem>0?'#dc2626':'#16a34a'};">${wft.wsRem>0?fmt(wft.wsRem,cur):'مسدد ✓'}</div><div class="kpi-l">المتبقي</div></div>
      <div class="kpi"><div class="kpi-v">${wks.length}</div><div class="kpi-l">عدد الورشات</div></div>
    </div>
    <!-- Workshop details -->
    <h2>تفاصيل الورشات وسجلات الدفع</h2>
    <table><thead><tr><th colspan="7">الورشات</th></tr></thead><tbody>${wsRows}</tbody></table>
    <p style="margin-top:20px;font-size:10px;color:#999;border-top:1px solid #eee;padding-top:8px;">
      ProjexID — ${esc(co.name||'')} — ${date}
    </p>
  
<script>
// ── Startup: check session then show login or app ──
(async function startApp() {
  await initDB();
  // Load dynamic users first
  try {
    const uSaved = localStorage.getItem('pxid_users');
    DUSERS = uSaved ? JSON.parse(uSaved) : null;
  } catch(e) { DUSERS = null; }

  const restored = tryRestoreSession();
  if (restored) {
    // Valid session — go straight to app
    await loadAllData();
    document.getElementById('login-wrap').style.display = 'none';
    document.getElementById('app').style.display = 'flex';
    applyRoleUI();
    renderAll();
  } else {
    // No session — show login
    document.getElementById('login-wrap').style.display = 'flex';
    document.getElementById('app').style.display = 'none';
  }
})();
</script>
</body></html>`);
  w.document.close();
  setTimeout(()=>w.print(),600);
}

// ── Print single workshop ─────────────────────────────────────────
function printSingleWorkshop(projId, wsId) {
  const p  = STATE.projects.find(x=>x.id===projId); if(!p) return;
  const ws = (p.workforce?.workshops||[]).find(x=>x.id===wsId); if(!ws) return;
  const c  = STATE.clients.find(cl=>cl.id===p.clientId);
  const fin= getProjFin(p);
  const cur= fin.currency||p.currency||'USD';
  const t  = TYPES[p.taskTypeKey]||{};
  const co = SETTINGS?.company||{};
  const total=spTotal(ws), paid=spPaid(ws), rem=total-paid;
  const pct = total?Math.round(paid/total*100):0;
  const date = new Date().toLocaleDateString('ar-SA');

  let runBal=0;
  const payRows = (ws.payments||[]).map((pm,i)=>{
    runBal+=pm.amount||0;
    const remaining=total-runBal;
    return `<tr>
      <td style="padding:7px 10px;">${i+1}</td>
      <td style="padding:7px 10px;">${payTypeLabel(pm.type)}</td>
      <td style="padding:7px 10px;">${pm.date||'—'}</td>
      <td style="padding:7px 10px;color:#16a34a;font-weight:700;">${fmt(pm.amount||0,cur)}</td>
      <td style="padding:7px 10px;">${payMethodLabel(pm.method)}</td>
      <td style="padding:7px 10px;">${esc(pm.ref||'—')}</td>
      <td style="padding:7px 10px;color:${remaining>0?'#dc2626':'#16a34a'};font-weight:700;">${fmt(Math.max(0,remaining),cur)}</td>
      <td style="padding:7px 10px;color:#888;">${esc(pm.notes||'')}</td>
    </tr>`;
  }).join('');

  const w = window.open('','_blank','width=820,height:1100');
  w.document.write(`<!DOCTYPE html><html dir="rtl" lang="ar"><head><meta charset="UTF-8">
    <title>كشف ورشة — ${esc(ws.name)}</title>
    <style>body{font-family:'Segoe UI',Tahoma,sans-serif;padding:24px;direction:rtl;color:#1c1c1a;}
    h1{font-size:18px;margin:0;}.section{background:#f5f5f5;border-radius:8px;padding:14px;margin:12px 0;}
    table{width:100%;border-collapse:collapse;font-size:12px;}td,th{border:1px solid #e5e7eb;padding:7px 10px;text-align:right;}
    th{background:#534AB7;color:#fff;}.total-row td{background:#ede9ff;font-weight:700;color:#534AB7;}
    @media print{body{padding:12px;}button{display:none;}}</style>
  </head><body>
    <div style="display:flex;justify-content:space-between;align-items:flex-start;border-bottom:3px solid #534AB7;padding-bottom:10px;margin-bottom:16px;">
      <div>
        <h1>🏭 كشف حساب ورشة</h1>
        <div style="font-size:13px;font-weight:700;color:#534AB7;margin-top:4px;">${esc(ws.name||'—')}</div>
        <div style="font-size:12px;color:#666;margin-top:3px;">
          <b>المشروع:</b> ${esc(p.projectCode)} &nbsp;|&nbsp;
          <b>العميل:</b> ${esc(c?.name||'—')} &nbsp;|&nbsp;
          <b>النوع:</b> ${t.icon||''} ${t.ar||''}
          ${p.propertyNumber?` &nbsp;|&nbsp; <b>رقم العقار:</b> ${esc(p.propertyNumber)}`:''}
          ${p.district?` &nbsp;|&nbsp; <b>المنطقة:</b> ${esc(p.district)}`:''}
        </div>
      </div>
      <button onclick="window.print()" style="padding:8px 16px;background:#534AB7;color:#fff;border:none;border-radius:6px;cursor:pointer;">🖨 طباعة</button>
    </div>
    <!-- Worksheet details -->
    <div class="section">
      <div style="display:grid;grid-template-columns:1fr 1fr 1fr;gap:10px;">
        <div><div style="font-size:10px;color:#888;">نوع العمل</div><div style="font-weight:700;">${esc(ws.type||'—')}</div></div>
        <div><div style="font-size:10px;color:#888;">البند المرتبط</div><div style="font-weight:700;">${esc(ws.item||'—')}</div></div>
        <div><div style="font-size:10px;color:#888;">المسؤول</div><div style="font-weight:700;">${esc(ws.manager||'—')}</div></div>
        <div><div style="font-size:10px;color:#888;">الهاتف</div><div style="font-weight:700;">${esc(ws.phone||'—')}</div></div>
        <div><div style="font-size:10px;color:#888;">الكمية × الوحدة</div><div style="font-weight:700;">${ws.qty||0} ${esc(ws.unit||'')} × ${fmt(ws.unitPrice||0,cur)}</div></div>
        <div><div style="font-size:10px;color:#888;">نسبة الإنجاز</div><div style="font-weight:700;">${ws.progress||0}%</div></div>
      </div>
    </div>
    <!-- Financial summary -->
    <div style="display:grid;grid-template-columns:repeat(3,1fr);gap:10px;margin:14px 0;">
      <div style="background:#ede9ff;border-radius:8px;padding:12px;text-align:center;">
        <div style="font-size:20px;font-weight:700;color:#534AB7;">${fmt(total,cur)}</div>
        <div style="font-size:10px;color:#888;margin-top:2px;">قيمة العقد الإجمالية</div>
      </div>
      <div style="background:#dcfce7;border-radius:8px;padding:12px;text-align:center;">
        <div style="font-size:20px;font-weight:700;color:#16a34a;">${fmt(paid,cur)}</div>
        <div style="font-size:10px;color:#888;margin-top:2px;">المدفوع (${pct}%)</div>
      </div>
      <div style="background:${rem>0?'#fee2e2':'#dcfce7'};border-radius:8px;padding:12px;text-align:center;">
        <div style="font-size:20px;font-weight:700;color:${rem>0?'#dc2626':'#16a34a'};">${rem>0?fmt(rem,cur):'مسدد ✓'}</div>
        <div style="font-size:10px;color:#888;margin-top:2px;">المتبقي</div>
      </div>
    </div>
    <!-- Payment ledger -->
    ${payRows ? `
    <h2 style="font-size:13px;color:#534AB7;border-bottom:2px solid #534AB7;padding-bottom:4px;margin:16px 0 10px;">
      سجل الدفعات (${ws.payments.length} دفعة)
    </h2>
    <table>
      <thead><tr><th>#</th><th>نوع الدفعة</th><th>التاريخ</th><th>المبلغ</th><th>طريقة الدفع</th><th>المرجع</th><th>الرصيد المتبقي</th><th>ملاحظات</th></tr></thead>
      <tbody>${payRows}
        <tr class="total-row">
          <td colspan="3">الإجمالي</td>
          <td>${fmt(paid,cur)}</td>
          <td colspan="2"></td>
          <td>${rem>0?fmt(rem,cur):'مسدد ✓'}</td>
          <td></td>
        </tr>
      </tbody>
    </table>` : '<div style="color:#888;font-size:12px;padding:10px 0;">لا توجد دفعات مسجّلة بعد</div>'}
    <p style="margin-top:24px;font-size:10px;color:#999;border-top:1px solid #eee;padding-top:8px;">
      ProjexID — ${esc(co.name||'')} — ${date}
    </p>
  
<script>
// ── Startup: check session then show login or app ──
(async function startApp() {
  await initDB();
  // Load dynamic users first
  try {
    const uSaved = localStorage.getItem('pxid_users');
    DUSERS = uSaved ? JSON.parse(uSaved) : null;
  } catch(e) { DUSERS = null; }

  const restored = tryRestoreSession();
  if (restored) {
    // Valid session — go straight to app
    await loadAllData();
    document.getElementById('login-wrap').style.display = 'none';
    document.getElementById('app').style.display = 'flex';
    applyRoleUI();
    renderAll();
  } else {
    // No session — show login
    document.getElementById('login-wrap').style.display = 'flex';
    document.getElementById('app').style.display = 'none';
  }
})();
</script>
</body></html>`);
  w.document.close();
  setTimeout(()=>w.print(),600);
}

// ── Engineer Tasks: switch view ──────────────────────────────────
function setEtView(view) {
  ET_VIEW = view;
  ['normal','byengineer'].forEach(v=>{
    document.getElementById('et-vbtn-'+v)?.classList.toggle('on', v===view);
  });
  const filterBar = document.getElementById('et-filter-bar');
  if(filterBar) filterBar.style.display = view==='normal' ? '' : 'none';
  document.getElementById('eng-tasks-list')?.style.setProperty('display', view==='normal'?'':'none');
  document.getElementById('eng-tasks-byeng')?.style.setProperty('display', view==='byengineer'?'':'none');
  if(view==='byengineer') renderEngTasksByEngineer();
}

// ── Render tasks grouped by engineer ─────────────────────────────
function renderEngTasksByEngineer() {
  const el = document.getElementById('eng-tasks-byeng');
  if(!el) return;

  // For engineer role: show only their projects
  const isMgr = CU?.role === 'manager';

  // Group projects by engineer
  const groups = {};
  STATE.projects.forEach(p => {
    const eng = STATE.engineers.find(e=>e.id===p.engineerId);
    // engineer role only sees their own
    if(!isMgr) {
      const myEng = STATE.engineers.find(e=>e.name===CU.name||e.username===CU.username);
      if(!myEng || p.engineerId !== myEng.id) return;
    }
    const key   = p.engineerId ? String(p.engineerId) : 'unassigned';
    const eName = eng ? eng.name : 'غير مسند';
    if(!groups[key]) groups[key] = { eng, name:eName, projects:[] };
    groups[key].projects.push(p);
  });

  const engList = Object.values(groups).sort((a,b)=>{
    if(a.eng===null) return 1;
    if(b.eng===null) return -1;
    return a.name.localeCompare(b.name);
  });

  if(!engList.length) {
    el.innerHTML='<div class="empty"><i class="ti ti-users"></i><p>لا توجد مهام مسندة لمهندسين</p></div>';
    return;
  }

  el.innerHTML = engList.map(group => {
    const initials = group.name.split(' ').map(w=>w[0]).slice(0,2).join('');
    const projRows = group.projects.map(p => {
      const c  = STATE.clients.find(cl=>cl.id===p.clientId);
      const t  = TYPES[p.taskTypeKey]||{};
      const s  = STATUS[p.status]||{ar:p.status, badge:''};
      const pr = PRI[p.priority]||{};
      const prog = p.tracking?.progress || p.progress || 0;
      const isExec = isExecType(p);
      return `<div class="eng-proj-row" onclick="openEngProject(${p.id})">
        <span class="eng-proj-code">${esc(p.projectCode)}</span>
        <div class="eng-proj-info">
          <span class="eng-proj-client">${esc(c?.name||'—')}</span>
          <span class="badge ${t.badge||''}" style="font-size:10px;">${t.icon||''} ${t.ar||''}</span>
          ${p.description?`<span class="eng-proj-desc">${esc(p.description)}</span>`:''}
        </div>
        <div class="eng-proj-right">
          <span class="badge ${s.badge}" style="font-size:10px;">${s.ar}</span>
          ${pr.ar?`<span class="badge ${pr.badge||''}" style="font-size:10px;">${pr.ar}</span>`:''}
          <div style="text-align:center;min-width:50px;">
            <div style="font-size:11px;font-weight:700;color:var(--accent);">${prog}%</div>
            <div style="width:50px;height:4px;background:var(--border);border-radius:2px;overflow:hidden;">
              <div style="width:${prog}%;height:100%;background:var(--accent);border-radius:2px;"></div>
            </div>
          </div>
          ${p.deliveryDate?`<span style="font-size:10.5px;color:var(--text3);">📅 ${p.deliveryDate}</span>`:''}
          <button class="eng-open-btn" onclick="event.stopPropagation();openEngProject(${p.id})">
            <i class="ti ti-folder-open"></i>
            ${isExec?'المتابعة':'التفاصيل'}
          </button>
        </div>
      </div>`;
    }).join('');

    return `<div class="eng-group-card">
      <div class="eng-group-hdr">
        <div style="display:flex;align-items:center;gap:12px;">
          <div class="eng-avatar-lg">${esc(initials||'؟')}</div>
          <div>
            <div class="eng-group-name">${esc(group.name)}</div>
            <div class="eng-group-sub">
              ${group.eng?.specialty||''} ${group.eng?.phone?'• 📞 '+group.eng.phone:''}
            </div>
          </div>
        </div>
        <div style="text-align:left;">
          <div style="font-size:22px;font-weight:700;">${group.projects.length}</div>
          <div style="font-size:11px;opacity:.75;">مشروع</div>
        </div>
      </div>
      <div>${projRows}</div>
    </div>`;
  }).join('');
}

// ── Open project from engineer view → followup or project detail ──
function openEngProject(projId) {
  const p = STATE.projects.find(x=>x.id===projId);
  if(!p) return;
  if(isExecType(p)) {
    // Open followup directly
    openFollowup(projId);
  } else {
    // Switch to projects view and open the work order modal
    sw('projects', document.querySelector('[data-view="projects"]'));
    setTimeout(()=>openEditWO(projId), 150);
  }
}

// ── Render a generic report card ─────────────────────────────────
function renderRepCard(r) {
  if(!r) return '';
  const proj = STATE.projects.find(p=>p.id===r.projectId);
  const eng  = STATE.engineers.find(e=>e.id===r.engineerId);
  const t    = TYPES[r.taskTypeKey||proj?.taskTypeKey]||{};
  const typeLabels = { daily_site:'سجل يومي',daily:'يومي',weekly:'أسبوعي',
    milestone:'مرحلي',final:'نهائي',issue:'مشكلة ميدانية' };
  const typeLbl = typeLabels[r.reportType]||r.reportType||'تقرير';
  return `<div class="dl-report-card">
    <div class="dl-report-header">
      <div>
        <div style="font-size:13px;font-weight:700;color:var(--accent);">${esc(r.projectCode||r.title||'—')}</div>
        <div style="font-size:11px;color:var(--text3);">${esc(r.clientName||'—')}</div>
      </div>
      <div style="display:flex;flex-direction:column;align-items:flex-end;gap:4px;">
        <span style="font-size:12px;font-weight:700;color:var(--text1);">📅 ${r.date||'—'}</span>
        <span class="badge badge-done" style="font-size:10px;">${typeLbl}</span>
      </div>
    </div>
    <div class="dl-report-meta">
      ${r.engineerName?`<span class="dl-report-meta-item"><i class="ti ti-hard-hat"></i>${esc(r.engineerName)}</span>`:''}
      ${r.workshop?`<span class="dl-report-meta-item"><i class="ti ti-building-warehouse"></i>${esc(r.workshop)}</span>`:''}
      ${r.status?`<span class="dl-report-meta-item"><i class="ti ti-info-circle"></i>${esc(r.status)}</span>`:''}
    </div>
    ${r.summary?`<div class="dl-report-body">${esc(r.summary)}</div>`:''}
    <div class="dl-report-actions">
      <button class="dl-action-btn" onclick="printDailyReport('${r.logId||r.id}','${r.projectId}')">
        <i class="ti ti-printer"></i> طباعة
      </button>
      ${proj?`<button class="dl-action-btn" onclick="openFollowup(${proj.id})">
        <i class="ti ti-folder-open"></i> فتح المشروع
      </button>`:''}
    </div>
  </div>`;
}

// ── Build a project summary row inside a group ───────────────────
function repProjBlock(p, reportsForProj, showOpenBtn) {
  const c     = STATE.clients.find(cl=>cl.id===p.clientId);
  const eng   = STATE.engineers.find(e=>e.id===p.engineerId);
  const t     = TYPES[p.taskTypeKey]||{};
  const s     = STATUS[p.status]||{ar:p.status,badge:''};
  const isExec= isExecType(p);
  const prog  = p.tracking?.progress||p.progress||0;

  const repSection = reportsForProj.length
    ? `<div class="rep-cards-row" style="padding:10px 12px;">${
        reportsForProj.map(r=>{
          try{ return r.reportType==='daily_site'?renderDailyLogCard(r):renderRepCard(r); }
          catch(e){ return ''; }
        }).join('')
      }</div>`
    : `<div style="padding:10px 16px;font-size:12px;color:var(--text3);">
         <i class="ti ti-report-off" style="vertical-align:-2px;margin-left:5px;"></i>
         لا توجد تقارير مرسلة لهذا المشروع بعد
       </div>`;

  return `<div class="rep-sub-group">
    <div class="rep-sub-header open" onclick="this.classList.toggle('open');
      this.nextElementSibling.classList.toggle('open');">
      <div style="display:flex;align-items:center;gap:10px;flex-wrap:wrap;">
        <span style="font-family:monospace;font-size:12px;font-weight:700;color:var(--accent);">${esc(p.projectCode)}</span>
        <span class="badge ${t.badge||''}" style="font-size:10px;">${t.icon||''} ${t.ar||''}</span>
        <span style="font-size:12.5px;color:var(--text1);">${esc(c?.name||'—')}</span>
        ${p.description?`<span style="font-size:11px;color:var(--text3);">${esc(p.description)}</span>`:''}
        ${eng?`<span style="font-size:11px;color:var(--text3);">👷 ${esc(eng.name)}</span>`:''}
      </div>
      <div style="display:flex;align-items:center;gap:8px;">
        <span class="badge ${s.badge}" style="font-size:10px;">${s.ar}</span>
        <div style="text-align:center;min-width:44px;">
          <div style="font-size:10px;font-weight:700;color:var(--accent);">${prog}%</div>
          <div style="width:44px;height:4px;background:var(--border);border-radius:2px;overflow:hidden;">
            <div style="width:${prog}%;height:100%;background:var(--accent);border-radius:2px;"></div>
          </div>
        </div>
        <span class="rep-count-badge" style="background:var(--blue-light);color:var(--blue);">
          ${reportsForProj.length} تقرير
        </span>
        <button class="dl-action-btn" style="font-size:11px;padding:5px 10px;"
          onclick="event.stopPropagation();openRepProject(${p.id})">
          <i class="ti ti-folder-open"></i>
          ${isExec?'المتابعة':'التفاصيل'}
        </button>
      </div>
    </div>
    <div class="rep-sub-body open">${repSection}</div>
  </div>`;
}

function openRepProject(projId) {
  const p = STATE.projects.find(x=>x.id===projId);
  if(!p) return;
  if(isExecType(p)) {
    openFollowup(projId);
  } else {
    sw('projects', document.querySelector('[data-view="projects"]'));
    setTimeout(()=>openEditWO(projId), 150);
  }
}
// Workshop type change — handles "add new" inline
async function fuSpTypeChange(wsId, selectEl) {
  if(selectEl.value === '__new__') {
    // Restore previous value while prompting
    const p = STATE.projects.find(x=>x.id===FU_CUR);
    const s = (p?.workforce?.workshops||[]).find(x=>x.id===wsId);
    if(s) selectEl.value = s.type || getWorkshopTypes()[0];

    // Show inline add form
    const existing = selectEl.closest('td');
    const inp = document.createElement('input');
    inp.placeholder = 'اسم نوع الورشة الجديد...';
    inp.className = 'wf-inp';
    inp.style.cssText = 'border:2px solid var(--accent);border-radius:4px;padding:5px 8px;width:150px;font-size:12px;font-family:inherit;';
    inp.onkeydown = async (e) => {
      if(e.key==='Enter') {
        const newType = inp.value.trim();
        if(!newType) { inp.remove(); return; }
        // Save to SETTINGS
        if(!SETTINGS.workshopTypes) SETTINGS.workshopTypes = [];
        if(!SETTINGS.workshopTypes.includes(newType)) {
          SETTINGS.workshopTypes.unshift(newType);
          await saveSettings();
        }
        // Set on workshop
        await fuSpField(wsId,'type',newType);
        toast('✓ تم إضافة نوع الورشة: '+newType);
        inp.remove();
      }
      if(e.key==='Escape') inp.remove();
    };
    existing.appendChild(inp);
    inp.focus();
    return;
  }
  await fuSpField(wsId,'type',selectEl.value);
}

// Also update fuSpAdd to use getWorkshopTypes()
// ══════════════════════════════════════════════════════════════════
// PHOTO COMMENT SYSTEM
// ══════════════════════════════════════════════════════════════════

// Migrate a photo entry: string → object
function migratePhoto(ph) {
  if(typeof ph === 'string') {
    return { id:'ph_'+Date.now()+'_'+Math.random().toString(36).slice(2,6),
             src:ph, caption:'', uploadedBy:'—', uploadedAt:0, comments:[] };
  }
  if(!ph.comments) ph.comments = [];
  return ph;
}

// Render a photo card with comment thread
function renderPhotoCard(ph, logId, phIdx) {
  ph = migratePhoto(ph);
  const timeStr = ph.uploadedAt
    ? new Date(ph.uploadedAt).toLocaleString('ar-SA',{dateStyle:'short',timeStyle:'short'})
    : '';
  const av = (ph.uploadedBy||'?').charAt(0);

  const commentsHtml = (ph.comments||[]).map((cm,ci)=>{
    const cmTime = cm.createdAt
      ? new Date(cm.createdAt).toLocaleString('ar-SA',{dateStyle:'short',timeStyle:'short'})
      : '';
    const roleClass = cm.role==='manager'?'mgr':cm.role==='engineer'?'eng':'';
    const cmAv = (cm.author||'؟').charAt(0);
    return `<div class="photo-comment-row">
      <div class="photo-comment-av ${roleClass}">${esc(cmAv)}</div>
      <div class="photo-comment-bubble">
        <div class="photo-comment-author">
          <span>${esc(cm.author||'مجهول')}</span>
          <button class="photo-comment-del" style="font-size:10px;padding:1px 5px;"
            onclick="fuPhotoCommentDel('${logId}','${ph.id}',${ci})"
            title="حذف"> حذف</button>
        </div>
        <div class="photo-comment-text">${esc(cm.text||'')}</div>
        <div class="photo-comment-time">${cmTime}</div>
      </div>
    </div>`;
  }).join('');

  const commentCount = (ph.comments||[]).length;

  return `<div class="photo-card" id="phcard-${ph.id}">
    <img class="photo-card-img" src="${ph.src}"
      onclick="showLightbox('${ph.src}')" alt="صورة موقع">
    <div class="photo-card-meta">
      <div class="photo-uploader-av">${esc(av)}</div>
      <span style="flex:1;font-weight:600;color:var(--text2);">${esc(ph.uploadedBy||'—')}</span>
      ${timeStr?`<span>${timeStr}</span>`:''}
      <button onclick="fuLogPhotoDel('${logId}',${phIdx})"
        style="background:rgba(220,38,38,.1);border:none;border-radius:50%;
               width:24px;height:24px;cursor:pointer;color:var(--red);
               display:flex;align-items:center;justify-content:center;font-size:13px;"> <i class="ti ti-trash" style="font-size:11px;"></i> حذف</button>
    </div>
    ${ph.caption?`<div style="padding:5px 12px;font-size:12px;color:var(--text2);">${esc(ph.caption)}</div>`:''}
    <div class="photo-comments">
      <div class="photo-comments-title">
        <i class="ti ti-message-circle"></i>
        التعليقات والملاحظات
        ${commentCount>0?`<span style="background:var(--accent);color:#fff;border-radius:10px;
          padding:1px 7px;font-size:10px;">${commentCount}</span>`:''}
      </div>
      ${commentsHtml || '<div style="font-size:11.5px;color:var(--text3);margin-bottom:8px;">لا توجد تعليقات بعد — كن أول من يعلق</div>'}
      <div class="photo-comment-input-row">
        <textarea class="photo-comment-inp" id="pcm-inp-${ph.id}" rows="1"
          placeholder="اكتب ملاحظة أو تعليقاً..."
          onkeydown="if(event.key==='Enter'&&!event.shiftKey){event.preventDefault();fuPhotoCommentAdd('${logId}','${ph.id}');}"></textarea>
        <button class="photo-comment-send"
          onclick="fuPhotoCommentAdd('${logId}','${ph.id}')">
          <i class="ti ti-send"></i>
        </button>
      </div>
    </div>
  </div>`;
}

// Add a comment to a photo
async function fuPhotoCommentAdd(logId, photoId) {
  const inp = document.getElementById('pcm-inp-'+photoId);
  const text = inp?.value.trim();
  if(!text) return;

  const p = STATE.projects.find(x=>x.id===FU_CUR);
  const L = (p?.tracking?.dailyLogs||[]).find(l=>l.id===logId);
  if(!L) return;
  // Migrate all photos
  L.photos = (L.photos||[]).map(migratePhoto);
  const ph = L.photos.find(x=>x.id===photoId);
  if(!ph) return;

  const comment = {
    id:        'cm_'+Date.now(),
    text,
    author:    CU.name || 'مجهول',
    role:      CU.role || 'viewer',
    avatar:    CU.avatar || '',
    createdAt: Date.now(),
  };
  ph.comments = ph.comments || [];
  ph.comments.push(comment);

  await fuSave();
  inp.value = '';
  fuRender(); // re-render to show new comment
}

// Delete a comment from a photo
async function fuPhotoCommentDel(logId, photoId, commentIdx) {
  if(!confirm('حذف هذا التعليق؟')) return;
  const p = STATE.projects.find(x=>x.id===FU_CUR);
  const L = (p?.tracking?.dailyLogs||[]).find(l=>l.id===logId);
  if(!L) return;
  L.photos = (L.photos||[]).map(migratePhoto);
  const ph = L.photos.find(x=>x.id===photoId);
  if(!ph) return;
  ph.comments.splice(commentIdx,1);
  await fuSave();
  fuRender();
}


// ═══════════════════════════════════════════════════════════════
// PROJECT FOLLOWUP — متابعة المشاريع
// ═══════════════════════════════════════════════════════════════

// State
let PF_PROJ_ID = null;
let PF_TASK_ID = null;
let PF_STAGE_ID= null;
let PF_VIEW    = 'list';  // list | kanban
let PF_DTAB    = 'details'; // details|checklist|comments|attachments|activity

// Constants
const PF_STATUSES = {
  new:      { ar:'جديد',           cls:'pf-s-new',      bcls:'pf-sb-new',      dot:'#9ca3af' },
  planned:  { ar:'مخطط',           cls:'pf-s-planned',  bcls:'pf-sb-planned',  dot:'#3b82f6' },
  inprog:   { ar:'قيد التنفيذ',    cls:'pf-s-inprog',   bcls:'pf-sb-inprog',   dot:'#8b5cf6' },
  review:   { ar:'بانتظار مراجعة', cls:'pf-s-review',   bcls:'pf-sb-review',   dot:'#f59e0b' },
  fix:      { ar:'بحاجة تصحيح',   cls:'pf-s-fix',      bcls:'pf-sb-fix',      dot:'#ef4444' },
  approved: { ar:'معتمد',          cls:'pf-s-approved', bcls:'pf-sb-approved', dot:'#10b981' },
  done:     { ar:'مكتمل',          cls:'pf-s-done',     bcls:'pf-sb-done',     dot:'#16a34a' },
  hold:     { ar:'متوقف',          cls:'pf-s-hold',     bcls:'pf-sb-hold',     dot:'#9ca3af' },
};
const PF_PRIORITIES = {
  urgent: { ar:'عاجل',   cls:'pf-pri-urgent', icon:'🔴' },
  high:   { ar:'عالية',  cls:'pf-pri-high',   icon:'🟠' },
  medium: { ar:'متوسطة', cls:'pf-pri-medium', icon:'🔵' },
  low:    { ar:'منخفضة', cls:'pf-pri-low',    icon:'⚪' },
};
const PF_STAGE_COLORS = ['#534AB7','#16a34a','#0d9488','#d97706','#dc2626','#7c3aed','#0891b2','#db2777'];
const PF_DEFAULT_STAGES = [
  'الأعمال التمهيدية','الحفريات','الأساسات','الهيكل الإنشائي','المباني','اللياسة','الكهرباء','السباكة','التشطيبات','التسليم'
];

// ── Data helpers ─────────────────────────────────────────────────
function pfUID(pfx){ return (pfx||'pf')+'-'+Date.now().toString(36)+Math.random().toString(36).slice(2,6); }

function pfEnsure(p) {
  if(!p.followup) p.followup = { stages:[] };
  if(!p.followup.stages || !p.followup.stages.length) {
    p.followup.stages = PF_DEFAULT_STAGES.map((name,i)=>({
      id:pfUID('stg'), name, order:i, color:PF_STAGE_COLORS[i%PF_STAGE_COLORS.length],
      tasks:[], collapsed:false
    }));
  }
  return p;
}

function pfGetProj()  { return STATE.projects.find(x=>x.id===PF_PROJ_ID); }
function pfGetStage() { const p=pfGetProj(); return p?.followup?.stages?.find(s=>s.id===PF_STAGE_ID); }
function pfGetTask()  {
  const p=pfGetProj();
  for(const st of (p?.followup?.stages||[])){
    const t=st.tasks?.find(t=>t.id===PF_TASK_ID);
    if(t) return {task:t, stage:st};
  }
  return null;
}

async function pfSave() {
  const p=pfGetProj(); if(!p) return;
  p.updatedAt=Date.now();
  await dbPut('projects', p);
}

function pfStageProgress(stage) {
  const tasks=stage.tasks||[];
  if(!tasks.length) return 0;
  const done=tasks.filter(t=>t.status==='done'||t.status==='approved').length;
  return Math.round(done/tasks.length*100);
}
function pfTaskProgress(task) {
  const cl=task.checklist||[];
  const sub=task.subtasks||[];
  const total=cl.length+sub.length;
  if(!total) return task.progress||0;
  const done=cl.filter(c=>c.done).length+sub.filter(s=>s.done).length;
  return Math.round(done/total*100);
}
function pfProjProgress(p) {
  const stages=p?.followup?.stages||[];
  if(!stages.length) return 0;
  const tots=stages.reduce((s,st)=>s+(st.tasks?.length||0),0);
  if(!tots) return 0;
  const done=stages.reduce((s,st)=>s+(st.tasks||[]).filter(t=>t.status==='done'||t.status==='approved').length,0);
  return Math.round(done/tots*100);
}

// ── Main render ──────────────────────────────────────────────────
function renderProjFollowup() {
  renderPFProjectList();
  if(PF_PROJ_ID) renderPFMain();
}

function renderPFProjectList() {
  const el=document.getElementById('pf-proj-items'); if(!el) return;
  const q=(document.getElementById('pf-search')?.value||'').toLowerCase();
  let projs=[...STATE.projects];
  if(q) projs=projs.filter(p=>(p.projectCode||'').toLowerCase().includes(q)||(p.description||'').toLowerCase().includes(q));
  if(!projs.length){ el.innerHTML='<div style="padding:20px;text-align:center;color:var(--text3);font-size:12px;">لا توجد مشاريع</div>'; return; }
  el.innerHTML=projs.map(p=>{
    const c=STATE.clients.find(cl=>cl.id===p.clientId);
    const t=TYPES[p.taskTypeKey]||{};
    const prog=pfProjProgress(pfEnsure(p));
    return `<div class="pf-proj-item ${p.id===PF_PROJ_ID?'on':''}" onclick="pfSelectProject(${p.id})">
      <div style="flex:1;min-width:0;">
        <div class="pf-proj-code">${esc(p.projectCode)}</div>
        <div class="pf-proj-name">${esc(p.description||'—')}</div>
        <div class="pf-proj-meta">${esc(c?.name||'—')} • ${t.icon||''} ${t.ar||''}</div>
        <div class="pf-proj-prog"><div class="pf-proj-prog-fill" style="width:${prog}%;"></div></div>
        <div style="font-size:10px;color:var(--text3);margin-top:2px;">${prog}% مكتمل</div>
      </div>
    </div>`;
  }).join('');
}

function pfSelectProject(id) {
  PF_PROJ_ID=id; PF_TASK_ID=null; PF_STAGE_ID=null;
  const p=STATE.projects.find(x=>x.id===id); if(!p) return;
  pfEnsure(p);
  renderPFProjectList();
  renderPFMain();
}

function renderPFMain() {
  const el=document.getElementById('pf-main'); if(!el) return;
  const p=pfGetProj(); if(!p){ el.innerHTML='<div class="empty"><p>اختر مشروعاً</p></div>'; return; }
  pfEnsure(p);
  const c=STATE.clients.find(cl=>cl.id===p.clientId);
  const t=TYPES[p.taskTypeKey]||{};
  const prog=pfProjProgress(p);

  const topbar=`<div class="pf-topbar">
    <div>
      <div style="font-size:15px;font-weight:800;">${esc(p.projectCode)} — ${esc(p.description||'')}</div>
      <div style="font-size:11px;color:var(--text3);">${esc(c?.name||'—')} • ${t.icon||''} ${t.ar||''} • إنجاز: ${prog}%</div>
    </div>
    <div style="display:flex;gap:8px;align-items:center;flex-wrap:wrap;">
      <div class="pf-view-btns">
        <button class="pf-view-btn ${PF_VIEW==='list'?'on':''}" onclick="pfSetView('list')"><i class="ti ti-list"></i> قائمة</button>
        <button class="pf-view-btn ${PF_VIEW==='kanban'?'on':''}" onclick="pfSetView('kanban')"><i class="ti ti-layout-columns"></i> Kanban</button>
      </div>
      <button class="fu-btn fu-btn-primary" style="font-size:12px;padding:7px 14px;" onclick="pfAddStage()">
        <i class="ti ti-plus"></i> إضافة مرحلة
      </button>
    </div>
  </div>`;

  if(PF_VIEW==='kanban') {
    el.innerHTML=topbar+renderPFKanban(p);
  } else {
    el.innerHTML=topbar+renderPFList(p);
  }
}

function pfSetView(v){ PF_VIEW=v; renderPFMain(); }

// ── LIST VIEW ────────────────────────────────────────────────────
function renderPFList(p) {
  return (p.followup.stages||[]).map((st,si)=>{
    const prog=pfStageProgress(st);
    const tasks=(st.tasks||[]).map((t,ti)=>renderPFTaskRow(p,st,t)).join('');
    const collapsed=st.collapsed;
    return `<div class="pf-stage" id="pfs-${st.id}">
      <div class="pf-stage-header" onclick="pfToggleStage('${st.id}')">
        <div class="pf-stage-name">
          <div class="pf-stage-dot" style="background:${st.color||'#534AB7'};"></div>
          <span>${esc(st.name)}</span>
          <span style="font-size:11px;font-weight:400;color:var(--text3);">${st.tasks?.length||0} مهمة</span>
          ${prog===100?'<span style="font-size:10px;background:#dcfce7;color:#16a34a;border-radius:10px;padding:1px 7px;">✓ مكتملة</span>':''}
        </div>
        <div style="display:flex;align-items:center;gap:8px;">
          <div style="width:80px;height:5px;background:var(--border);border-radius:3px;overflow:hidden;">
            <div style="width:${prog}%;height:100%;background:${st.color||'#534AB7'};border-radius:3px;"></div>
          </div>
          <span style="font-size:11px;font-weight:700;color:${st.color||'#534AB7'};">${prog}%</span>
          <div class="pf-stage-actions" onclick="event.stopPropagation()">
            <button class="fu-btn" style="font-size:11px;padding:4px 8px;" onclick="pfEditStage('${st.id}')"><i class="ti ti-pencil"></i> تعديل</button>
            <button class="fu-btn" style="font-size:11px;padding:4px 8px;" onclick="pfMoveStage('${st.id}',-1)" title="للأعلى"><i class="ti ti-arrow-up"></i> أعلى</button>
            <button class="fu-btn" style="font-size:11px;padding:4px 8px;" onclick="pfMoveStage('${st.id}',1)" title="للأسفل"><i class="ti ti-arrow-down"></i> أسفل</button>
            <button class="fu-btn fu-btn-danger" style="font-size:11px;padding:4px 8px;" onclick="pfDeleteStage('${st.id}')"><i class="ti ti-trash"></i> حذف</button>
          </div>
          <i class="ti ti-chevron-${collapsed?'left':'down'}" style="font-size:14px;color:var(--text3);"></i>
        </div>
      </div>
      ${collapsed?'':(`<div class="pf-stage-body">
        ${tasks||'<div style="color:var(--text3);font-size:12px;padding:4px 0;">لا توجد مهام — أضف مهمة أدناه</div>'}
        <div class="pf-add-task" onclick="pfAddTask('${st.id}')"><i class="ti ti-plus" style="font-size:14px;"></i> إضافة مهمة</div>
      </div>`)}
    </div>`;
  }).join('')||'<div class="empty"><i class="ti ti-layout-list"></i><p>لا توجد مراحل — أضف مرحلة من الأعلى</p></div>';
}

function renderPFTaskRow(p, st, t) {
  const s=PF_STATUSES[t.status]||PF_STATUSES.new;
  const pr=PF_PRIORITIES[t.priority]||PF_PRIORITIES.medium;
  const cl=t.checklist||[]; const clDone=cl.filter(c=>c.done).length;
  const sub=t.subtasks||[]; const subDone=sub.filter(s=>s.done).length;
  const isDone=t.status==='done'||t.status==='approved';
  const eng=t.assigneeId?STATE.engineers.find(e=>e.id===t.assigneeId):null;
  return `<div class="pf-task ${t.id===PF_TASK_ID?'on':''}" id="pft-${t.id}" onclick="pfOpenTask('${st.id}','${t.id}')">
    <div class="pf-task-status ${s.cls}" style="border-radius:50%;background:${isDone?s.dot:'transparent'};border-color:${s.dot};"></div>
    <div class="pf-task-name ${isDone?'done':''}">${esc(t.name)}</div>
    <div class="pf-task-meta">
      ${t.dueDate?`<span style="font-size:10px;color:${new Date(t.dueDate)<new Date()&&!isDone?'var(--red)':'var(--text3)'};">📅 ${t.dueDate}</span>`:''}
      <span class="pf-task-pill ${s.bcls}">${s.ar}</span>
      <span style="font-size:11px;" title="${pr.ar}">${pr.icon}</span>
      ${cl.length?`<span style="font-size:10px;color:var(--text3);">☑ ${clDone}/${cl.length}</span>`:''}
      ${eng?`<span style="font-size:10px;color:var(--text3);">👷 ${esc(eng.name.split(' ')[0])}</span>`:''}
      ${(t.comments||[]).length?`<span style="font-size:10px;color:var(--text3);">💬 ${t.comments.length}</span>`:''}
    </div>
  </div>`;
}

// ── KANBAN VIEW ──────────────────────────────────────────────────
function renderPFKanban(p) {
  const allTasks=[];
  (p.followup.stages||[]).forEach(st=>(st.tasks||[]).forEach(t=>allTasks.push({task:t,stage:st})));
  const cols=['new','planned','inprog','review','fix','approved','done','hold'];
  return `<div class="pf-kanban">
    ${cols.map(sc=>{
      const s=PF_STATUSES[sc];
      const tasks=allTasks.filter(({task})=>task.status===sc);
      return `<div class="pf-kanban-col">
        <div class="pf-kanban-title ${s.bcls}">${s.ar} <span style="opacity:.7;">(${tasks.length})</span></div>
        ${tasks.map(({task,stage})=>`
          <div class="pf-kanban-card" onclick="pfOpenTask('${stage.id}','${task.id}')">
            <div style="font-size:11px;color:${stage.color};font-weight:700;margin-bottom:4px;">${esc(stage.name)}</div>
            <div style="font-size:12.5px;font-weight:600;color:var(--text1);">${esc(task.name)}</div>
            ${task.dueDate?`<div style="font-size:10.5px;color:var(--text3);margin-top:4px;">📅 ${task.dueDate}</div>`:''}
            ${(task.checklist||[]).length?`<div style="font-size:10px;color:var(--text3);margin-top:3px;">☑ ${task.checklist.filter(c=>c.done).length}/${task.checklist.length}</div>`:''}
          </div>`).join('')}
        <div class="pf-add-task" onclick="pfAddTaskKanban('${sc}')"><i class="ti ti-plus"></i> إضافة مهمة</div>
      </div>`;
    }).join('')}
  </div>`;
}

// ── STAGE OPERATIONS ─────────────────────────────────────────────
async function pfAddStage() {
  const name=prompt('اسم المرحلة الجديدة:'); if(!name?.trim()) return;
  const p=pfGetProj(); if(!p) return;
  p.followup.stages.push({
    id:pfUID('stg'), name:name.trim(), order:p.followup.stages.length,
    color:PF_STAGE_COLORS[p.followup.stages.length%PF_STAGE_COLORS.length],
    tasks:[], collapsed:false
  });
  await pfSave(); renderPFMain();
  logActivity('إضافة مرحلة: '+name);
}
async function pfEditStage(sid) {
  const p=pfGetProj(); if(!p) return;
  const st=p.followup.stages.find(s=>s.id===sid); if(!st) return;
  const name=prompt('اسم المرحلة:',st.name); if(!name?.trim()) return;
  st.name=name.trim();
  await pfSave(); renderPFMain();
}
async function pfDeleteStage(sid) {
  const p=pfGetProj(); if(!p) return;
  const st=p.followup.stages.find(s=>s.id===sid); if(!st) return;
  if(st.tasks?.length && !confirm(`حذف مرحلة "${st.name}" مع ${st.tasks.length} مهمة؟`)) return;
  p.followup.stages=p.followup.stages.filter(s=>s.id!==sid);
  await pfSave(); renderPFMain();
}
async function pfMoveStage(sid, dir) {
  const p=pfGetProj(); if(!p) return;
  const stages=p.followup.stages;
  const i=stages.findIndex(s=>s.id===sid); if(i<0) return;
  const ni=i+dir; if(ni<0||ni>=stages.length) return;
  [stages[i],stages[ni]]=[stages[ni],stages[i]];
  await pfSave(); renderPFMain();
}
function pfToggleStage(sid) {
  const p=pfGetProj(); if(!p) return;
  const st=p.followup.stages.find(s=>s.id===sid); if(!st) return;
  st.collapsed=!st.collapsed;
  renderPFMain();
}

// ── TASK OPERATIONS ──────────────────────────────────────────────
async function pfAddTask(sid) {
  const name=prompt('اسم المهمة:'); if(!name?.trim()) return;
  const p=pfGetProj(); if(!p) return;
  const st=p.followup.stages.find(s=>s.id===sid); if(!st) return;
  if(!st.tasks) st.tasks=[];
  const task={
    id:pfUID('tsk'), name:name.trim(), description:'',
    status:'new', priority:'medium',
    startDate:'', dueDate:'', progress:0,
    assigneeId:null, workshop:'', tags:[], notes:'',
    subtasks:[], checklist:[], comments:[], attachments:[], activity:[],
    createdAt:Date.now(), updatedAt:Date.now()
  };
  st.tasks.push(task);
  await pfSave();
  logActivity('إضافة مهمة: '+name);
  renderPFMain();
}
async function pfAddTaskKanban(status) {
  const p=pfGetProj(); if(!p) return;
  const stages=p.followup.stages||[];
  if(!stages.length){ toast('⚠ أضف مرحلة أولاً'); return; }
  const sid=stages[0].id;
  const name=prompt('اسم المهمة:'); if(!name?.trim()) return;
  if(!stages[0].tasks) stages[0].tasks=[];
  stages[0].tasks.push({
    id:pfUID('tsk'), name:name.trim(), description:'',
    status, priority:'medium', startDate:'', dueDate:'', progress:0,
    assigneeId:null, workshop:'', tags:[], notes:'',
    subtasks:[], checklist:[], comments:[], attachments:[], activity:[],
    createdAt:Date.now(), updatedAt:Date.now()
  });
  await pfSave(); renderPFMain();
}

// ── TASK DRAWER ──────────────────────────────────────────────────
const PF_TABS=[
  {id:'details',    ar:'التفاصيل'},
  {id:'checklist',  ar:'Checklist'},
  {id:'comments',   ar:'النقاش'},
  {id:'attachments',ar:'المرفقات'},
  {id:'activity',   ar:'النشاط'},
];

function pfOpenTask(sid, tid) {
  PF_STAGE_ID=sid; PF_TASK_ID=tid; PF_DTAB='details';
  const drawer=document.getElementById('pf-drawer');
  if(drawer) drawer.classList.add('open');
  pfRenderDrawer();
}
function pfCloseTask() {
  PF_TASK_ID=null; PF_STAGE_ID=null;
  document.getElementById('pf-drawer')?.classList.remove('open');
  renderPFMain();
}

function pfRenderDrawer() {
  const res=pfGetTask(); if(!res) return;
  const {task:t, stage:st}=res;
  const s=PF_STATUSES[t.status]||PF_STATUSES.new;
  const pr=PF_PRIORITIES[t.priority]||PF_PRIORITIES.medium;
  document.getElementById('pf-dt-status-badge').innerHTML=`<span class="pf-task-pill ${s.bcls}" style="font-size:11px;">${s.ar}</span>`;
  document.getElementById('pf-dt-name').textContent=t.name;
  document.getElementById('pf-dt-meta').textContent=`${esc(st.name)} • ${pr.icon} ${pr.ar}${t.dueDate?' • 📅 '+t.dueDate:''}`;
  // Tabs
  document.getElementById('pf-drawer-tabs').innerHTML=PF_TABS.map(tab=>
    `<div class="pf-dtab ${tab.id===PF_DTAB?'on':''}" onclick="pfSetDTab('${tab.id}')">${tab.ar}</div>`
  ).join('');
  // Body
  pfRenderDTabBody(t, st);
}

function pfSetDTab(tab){ PF_DTAB=tab; pfRenderDrawer(); }

function pfRenderDTabBody(t, st) {
  const el=document.getElementById('pf-drawer-body'); if(!el) return;
  const p=pfGetProj();
  if(PF_DTAB==='details')    el.innerHTML=pfTabDetails(t, st, p);
  if(PF_DTAB==='checklist')  el.innerHTML=pfTabChecklist(t);
  if(PF_DTAB==='comments')   el.innerHTML=pfTabComments(t);
  if(PF_DTAB==='attachments')el.innerHTML=pfTabAttachments(t);
  if(PF_DTAB==='activity')   el.innerHTML=pfTabActivity(t);
}

function pfTabDetails(t, st, p) {
  const engs=STATE.engineers||[];
  return `<div style="display:flex;flex-direction:column;gap:12px;">
    <div class="fg"><label>اسم المهمة</label>
      <input class="fi" value="${esc(t.name)}" onchange="pfTaskField('${t.id}','name',this.value)"></div>
    <div class="fg"><label>الوصف</label>
      <textarea class="fi" rows="3" placeholder="وصف المهمة..." onchange="pfTaskField('${t.id}','description',this.value)">${esc(t.description||'')}</textarea></div>
    <div class="frow">
      <div class="fg"><label>الحالة</label>
        <select class="fi" onchange="pfTaskField('${t.id}','status',this.value)">
          ${Object.entries(PF_STATUSES).map(([k,v])=>`<option value="${k}" ${t.status===k?'selected':''}>${v.ar}</option>`).join('')}
        </select></div>
      <div class="fg"><label>الأولوية</label>
        <select class="fi" onchange="pfTaskField('${t.id}','priority',this.value)">
          ${Object.entries(PF_PRIORITIES).map(([k,v])=>`<option value="${k}" ${t.priority===k?'selected':''}>${v.icon} ${v.ar}</option>`).join('')}
        </select></div>
    </div>
    <div class="frow">
      <div class="fg"><label>تاريخ البداية</label>
        <input class="fi" type="date" value="${t.startDate||''}" onchange="pfTaskField('${t.id}','startDate',this.value)"></div>
      <div class="fg"><label>تاريخ الاستحقاق</label>
        <input class="fi" type="date" value="${t.dueDate||''}" onchange="pfTaskField('${t.id}','dueDate',this.value)"></div>
    </div>
    <div class="fg"><label>المهندس المسؤول</label>
      <select class="fi" onchange="pfTaskField('${t.id}','assigneeId',this.value?parseInt(this.value):null)">
        <option value="">— بدون تعيين —</option>
        ${engs.map(e=>`<option value="${e.id}" ${t.assigneeId===e.id?'selected':''}>${esc(e.name)}</option>`).join('')}
      </select></div>
    <div class="fg"><label>الورشة المسؤولة</label>
      <select class="fi" onchange="pfTaskField('${t.id}','workshop',this.value)">
        <option value="">— بدون ورشة —</option>
        ${getWorkshopTypes().map(ws=>`<option ${t.workshop===ws?'selected':''}>${esc(ws)}</option>`).join('')}
      </select></div>
    <div class="fg"><label>ملاحظات</label>
      <textarea class="fi" rows="3" placeholder="ملاحظات..." onchange="pfTaskField('${t.id}','notes',this.value)">${esc(t.notes||'')}</textarea></div>
    <div style="display:flex;gap:8px;margin-top:4px;">
      <button class="btn-cancel" style="font-size:12px;" onclick="pfDeleteTask('${st.id}','${t.id}')">
        <i class="ti ti-trash"></i> حذف المهمة
      </button>
    </div>
  </div>`;
}

function pfTabChecklist(t) {
  const cl=t.checklist||[];
  const done=cl.filter(c=>c.done).length;
  const pct=cl.length?Math.round(done/cl.length*100):0;
  return `<div>
    <div style="font-size:12px;color:var(--text3);margin-bottom:10px;display:flex;justify-content:space-between;">
      <span>☑ ${done}/${cl.length} مكتمل</span>
      <span style="font-weight:700;color:var(--accent);">${pct}%</span>
    </div>
    <div style="height:5px;background:var(--border);border-radius:3px;margin-bottom:14px;overflow:hidden;">
      <div style="width:${pct}%;height:100%;background:var(--accent);border-radius:3px;"></div>
    </div>
    ${cl.map((c,i)=>`<div style="display:flex;align-items:center;gap:8px;padding:7px 0;border-bottom:1px solid var(--border);">
      <input type="checkbox" ${c.done?'checked':''} style="width:16px;height:16px;accent-color:var(--accent);"
        onchange="pfChecklistToggle('${t.id}',${i},this.checked)">
      <span style="flex:1;font-size:13px;color:${c.done?'var(--text3)':'var(--text1)'};${c.done?'text-decoration:line-through;':''}">
        ${esc(c.text)}</span>
      <button onclick="pfChecklistDel('${t.id}',${i})" style="background:none;border:none;cursor:pointer;color:var(--text3);font-size:12px;padding:2px 5px;">
        <i class="ti ti-trash"></i> حذف</button>
    </div>`).join('')}
    <div style="display:flex;gap:8px;margin-top:10px;">
      <input class="fi" id="pf-cl-inp" placeholder="إضافة بند..." style="flex:1;"
        onkeydown="if(event.key==='Enter')pfChecklistAdd('${t.id}')">
      <button class="btn-save" style="font-size:12px;padding:7px 14px;" onclick="pfChecklistAdd('${t.id}')">
        <i class="ti ti-plus"></i> إضافة</button>
    </div>
  </div>`;
}

function pfTabComments(t) {
  const comments=t.comments||[];
  const commHtml=comments.map((cm,i)=>`
    <div class="pf-comment">
      <div class="pf-comment-av" style="background:${cm.role==='manager'?'#534AB7':'#16a34a'};">${(cm.author||'?').charAt(0)}</div>
      <div class="pf-comment-bubble">
        <div class="pf-comment-meta">
          <span class="pf-comment-author">${esc(cm.author||'مجهول')}</span>
          <div style="display:flex;align-items:center;gap:6px;">
            <span>${new Date(cm.createdAt||0).toLocaleString('ar-SA',{dateStyle:'short',timeStyle:'short'})}</span>
            <button onclick="pfCommentDel('${t.id}',${i})" style="background:none;border:none;cursor:pointer;color:var(--text3);font-size:11px;padding:1px 4px;">
              <i class="ti ti-trash"></i> حذف</button>
          </div>
        </div>
        <div class="pf-comment-text">${esc(cm.text||'')}</div>
      </div>
    </div>`).join('')||'<div style="color:var(--text3);font-size:12px;margin-bottom:14px;">لا توجد تعليقات — ابدأ النقاش</div>';
  return `<div>
    ${commHtml}
    <div style="margin-top:10px;">
      <textarea class="pf-comment-inp" id="pf-cm-inp" placeholder="اكتب تعليقاً أو ملاحظة..."
        onkeydown="if(event.key==='Enter'&&event.ctrlKey)pfCommentAdd('${t.id}')"></textarea>
      <div style="font-size:10.5px;color:var(--text3);margin:4px 0 8px;">Ctrl+Enter للإرسال</div>
      <button class="btn-save" style="font-size:12px;padding:7px 18px;" onclick="pfCommentAdd('${t.id}')">
        <i class="ti ti-send"></i> إرسال التعليق</button>
    </div>
  </div>`;
}

function pfTabAttachments(t) {
  const atts=t.attachments||[];
  return `<div>
    <label class="fu-btn fu-btn-primary" style="display:inline-flex;align-items:center;gap:6px;cursor:pointer;">
      <i class="ti ti-upload"></i> رفع ملف أو صورة
      <input type="file" multiple style="display:none;" onchange="pfUploadAttachment('${t.id}',this)">
    </label>
    <label class="fu-btn-cam" style="display:inline-flex;align-items:center;gap:6px;cursor:pointer;margin-right:8px;">
      <i class="ti ti-camera"></i> كاميرا
      <input type="file" accept="image/*" capture="environment" style="display:none;" onchange="pfUploadAttachment('${t.id}',this)">
    </label>
    <div style="margin-top:12px;">
      ${atts.map((a,i)=>`<div style="display:flex;align-items:center;gap:8px;padding:8px 0;border-bottom:1px solid var(--border);">
        <i class="ti ti-file" style="color:var(--accent);font-size:20px;"></i>
        <div style="flex:1;min-width:0;">
          <div style="font-size:12.5px;font-weight:600;overflow:hidden;text-overflow:ellipsis;white-space:nowrap;">${esc(a.name)}</div>
          <div style="font-size:10.5px;color:var(--text3);">${esc(a.uploadedBy||'—')} • ${a.uploadedAt?new Date(a.uploadedAt).toLocaleDateString('ar-SA'):''}</div>
        </div>
        ${a.type?.startsWith('image/')?`<button onclick="showLightbox('${a.data}')" style="background:none;border:none;cursor:pointer;color:var(--blue);font-size:12px;"><i class="ti ti-eye"></i> عرض</button>`:''}
        <a href="${a.data||''}" download="${a.name||'file'}" style="font-size:12px;color:var(--accent);text-decoration:none;"><i class="ti ti-download"></i> تحميل</a>
        <button onclick="pfDeleteAttachment('${t.id}',${i})" style="background:none;border:none;cursor:pointer;color:var(--red);font-size:12px;"><i class="ti ti-trash"></i> حذف</button>
      </div>`).join('')||'<div style="color:var(--text3);font-size:12px;padding:8px 0;">لا توجد مرفقات</div>'}
    </div>
  </div>`;
}

function pfTabActivity(t) {
  const acts=(t.activity||[]).slice().reverse();
  return `<div>${acts.map(a=>`
    <div style="display:flex;gap:8px;padding:8px 0;border-bottom:1px solid var(--border);">
      <div style="width:8px;height:8px;border-radius:50%;background:var(--accent);margin-top:5px;flex-shrink:0;"></div>
      <div>
        <span style="font-weight:700;color:var(--accent);">${esc(a.user||'—')}</span>
        <span style="color:var(--text2);"> ${esc(a.detail||'')}</span>
        <div style="font-size:10.5px;color:var(--text3);">${new Date(a.time||0).toLocaleString('ar-SA',{dateStyle:'short',timeStyle:'short'})}</div>
      </div>
    </div>`).join('')||'<div style="color:var(--text3);font-size:12px;padding:8px 0;">لا يوجد نشاط مسجّل</div>'}
  </div>`;
}

// ── TASK DATA OPERATIONS ─────────────────────────────────────────
async function pfTaskField(tid, key, val) {
  const p=pfGetProj(); if(!p) return;
  for(const st of (p.followup.stages||[])){
    const t=st.tasks?.find(t=>t.id===tid); if(!t) continue;
    t[key]=val; t.updatedAt=Date.now();
    pfAddActivity(t, `تعديل الحقل: ${key} → ${val}`);
    await pfSave();
    pfRenderDrawer();
    return;
  }
}
async function pfDeleteTask(sid, tid) {
  if(!confirm('حذف هذه المهمة؟')) return;
  const p=pfGetProj(); if(!p) return;
  const st=p.followup.stages.find(s=>s.id===sid); if(!st) return;
  st.tasks=st.tasks.filter(t=>t.id!==tid);
  await pfSave();
  pfCloseTask();
}
async function pfChecklistToggle(tid, idx, val) {
  const p=pfGetProj(); if(!p) return;
  for(const st of (p.followup.stages||[])){
    const t=st.tasks?.find(t=>t.id===tid); if(!t) continue;
    if(!t.checklist) t.checklist=[];
    t.checklist[idx].done=val;
    t.updatedAt=Date.now();
    await pfSave();
    pfRenderDrawer();
    return;
  }
}
async function pfChecklistAdd(tid) {
  const inp=document.getElementById('pf-cl-inp');
  const text=inp?.value.trim(); if(!text) return;
  const p=pfGetProj(); if(!p) return;
  for(const st of (p.followup.stages||[])){
    const t=st.tasks?.find(t=>t.id===tid); if(!t) continue;
    if(!t.checklist) t.checklist=[];
    t.checklist.push({id:pfUID('cl'),text,done:false});
    t.updatedAt=Date.now();
    await pfSave();
    inp.value='';
    pfRenderDrawer();
    return;
  }
}
async function pfChecklistDel(tid, idx) {
  const p=pfGetProj(); if(!p) return;
  for(const st of (p.followup.stages||[])){
    const t=st.tasks?.find(t=>t.id===tid); if(!t) continue;
    t.checklist.splice(idx,1); t.updatedAt=Date.now();
    await pfSave(); pfRenderDrawer(); return;
  }
}
async function pfCommentAdd(tid) {
  const inp=document.getElementById('pf-cm-inp');
  const text=inp?.value.trim(); if(!text) return;
  const p=pfGetProj(); if(!p) return;
  for(const st of (p.followup.stages||[])){
    const t=st.tasks?.find(t=>t.id===tid); if(!t) continue;
    if(!t.comments) t.comments=[];
    t.comments.push({id:pfUID('cm'),text,author:CU?.name||'مجهول',role:CU?.role||'viewer',createdAt:Date.now()});
    t.updatedAt=Date.now();
    pfAddActivity(t,'أضاف تعليقاً');
    await pfSave();
    inp.value='';
    pfRenderDrawer();
    return;
  }
}
async function pfCommentDel(tid, idx) {
  if(!confirm('حذف التعليق؟')) return;
  const p=pfGetProj(); if(!p) return;
  for(const st of (p.followup.stages||[])){
    const t=st.tasks?.find(t=>t.id===tid); if(!t) continue;
    t.comments.splice(idx,1); t.updatedAt=Date.now();
    await pfSave(); pfRenderDrawer(); return;
  }
}
async function pfUploadAttachment(tid, inp) {
  const p=pfGetProj(); if(!p) return;
  let task=null;
  for(const st of (p.followup.stages||[])){
    task=st.tasks?.find(t=>t.id===tid); if(task) break;
  }
  if(!task) return;
  if(!task.attachments) task.attachments=[];
  for(const file of Array.from(inp.files)){
    if(file.size>5*1024*1024){toast('⚠ الملف أكبر من 5MB');continue;}
    await new Promise(res=>{
      const r=new FileReader();
      r.onload=async e=>{
        task.attachments.push({id:pfUID('att'),name:file.name,type:file.type,data:e.target.result,size:file.size,uploadedBy:CU?.name||'—',uploadedAt:Date.now()});
        res();
      };
      r.readAsDataURL(file);
    });
  }
  task.updatedAt=Date.now();
  pfAddActivity(task,'رفع مرفق');
  await pfSave();
  inp.value='';
  pfRenderDrawer();
  toast('✓ تم رفع الملف');
}
async function pfDeleteAttachment(tid, idx) {
  if(!confirm('حذف هذا المرفق؟')) return;
  const p=pfGetProj(); if(!p) return;
  for(const st of (p.followup.stages||[])){
    const t=st.tasks?.find(t=>t.id===tid); if(!t) continue;
    t.attachments.splice(idx,1); t.updatedAt=Date.now();
    await pfSave(); pfRenderDrawer(); return;
  }
}
function pfAddActivity(task, detail) {
  if(!task.activity) task.activity=[];
  task.activity.push({id:pfUID('act'),user:CU?.name||'—',detail,time:Date.now()});
}

// ══════════════════════════════════════════════════════════════════
// GLOBAL SEARCH
// ══════════════════════════════════════════════════════════════════
function globalSearch() {
  const q = document.getElementById('gsearch').value.toLowerCase();
  if(!q) return;
  // Switch to projects and filter
  document.getElementById('proj-search').value = q;
  sw('projects', document.querySelector('.ni[data-view=projects]'));
  renderProjects();
}

// ══════════════════════════════════════════════════════════════════
// HELPERS
// ══════════════════════════════════════════════════════════════════
function esc(s) { return String(s||'').replace(/&/g,'&amp;').replace(/</g,'&lt;').replace(/>/g,'&gt;').replace(/"/g,'&quot;'); }
function fmtDate(ts) {
  if(!ts) return '';
  const d = new Date(ts);
  const months=['يناير','فبراير','مارس','أبريل','مايو','يونيو','يوليو','أغسطس','سبتمبر','أكتوبر','نوفمبر','ديسمبر'];
  return d.getDate()+' '+months[d.getMonth()]+' '+d.getFullYear();
}

let toastTimer;
function toast(msg) {
  const el = document.getElementById('toast');
  el.textContent = msg;
  el.classList.add('show');
  clearTimeout(toastTimer);
  toastTimer = setTimeout(()=>el.classList.remove('show'), 2600);
}

// ══════════════════════════════════════════════════════════════════
// KEYBOARD
// ══════════════════════════════════════════════════════════════════
document.addEventListener('keydown', e => {
  if(e.key==='Escape') {
    document.querySelectorAll('.overlay.open').forEach(o=>o.classList.remove('open'));
  }
});

// ══════════════════════════════════════════════════════════════════
// FOLLOWUP / TRACKING SYSTEM
// ══════════════════════════════════════════════════════════════════
const FU_DESIGN_PHASES = [
  {key:'requirements', name:'استلام المتطلبات'},
  {key:'architectural', name:'التصميم المعماري'},
  {key:'structural', name:'التصميم الإنشائي'},
  {key:'electrical', name:'التصميم الكهربائي'},
  {key:'mechanical', name:'التصميم الميكانيكي'},
  {key:'clientreview', name:'مراجعة العميل'},
  {key:'delivery', name:'التسليم النهائي'},
];
const FU_EXEC_STAGES = [
  {key:'prep', name:'الأعمال التمهيدية', checklist:['استلام الموقع','تنظيف الموقع','تسوير الموقع','مكتب الموقع','الخدمات المؤقتة','السلامة','اعتماد خطة التنفيذ']},
  {key:'excavation', name:'الحفريات', checklist:['الحفر','نقل المخلفات','تسوية القاع','الدمك','اختبار التربة','اعتماد المهندس']},
  {key:'foundations', name:'القواعد', checklist:['طبقة النظافة','الحدادة','النجارة','تمديدات أرضية','الصب','الاختبارات','المعالجة']},
  {key:'columns', name:'الأعمدة', checklist:['التسليح','النجارة','الفحص','الصب','المعالجة','فك القوالب']},
  {key:'beams', name:'الجسور', checklist:['الشدات','الحدادة','التمديدات','الفحص','الصب','المعالجة']},
  {key:'slabs', name:'الأسقف', checklist:['الشدات','التسليح','فتحات الخدمات','الفحص','الصب','المعالجة','فك القوالب']},
  {key:'walls', name:'الجدران والبلوك', checklist:['البلوك','الفتحات','ضبط الاستقامة','مراجعة الجودة']},
  {key:'electric', name:'الكهرباء', checklist:['مراجعة المخططات','تمديد المواسير','تمديد العلب','تمديد الكابلات','لوحات الكهرباء','القواطع','نقاط الإنارة','المفاتيح','المقابس','اختبار العزل','اختبار التشغيل','اعتماد المهندس']},
  {key:'plumb', name:'السباكة', checklist:['تمديد التغذية','تمديد الصرف','مياه ساخنة','مياه باردة','غرف التفتيش','اختبار الضغط','اختبار التسريب','اعتماد المهندس']},
  {key:'hvac', name:'التكييف', checklist:['الدكت','العوازل','الوحدات','النحاس','الصرف','الكهرباء','اختبار الضغط','اختبار التشغيل','اعتماد المهندس']},
  {key:'plaster', name:'اللياسة', checklist:['تنظيف الأسطح','معالجة الفواصل','شبك اللياسة','ضبط الزوايا','تجهيز الخلطات','اللياسة الداخلية','اللياسة الخارجية','ضبط السماكات','المعالجة','فحص الجودة','اعتماد المهندس']},
  {key:'paint', name:'معجون الجدران والدهانات', checklist:['تنظيف الأسطح','معالجة العيوب','صنفرة أولية','تطبيق المعجون','صنفرة نهائية','برايمر','الدهان الأول','الدهان الثاني','الدهان النهائي','معالجة العيوب','تنظيف','فحص الجودة','اعتماد المهندس']},
  {key:'tiles', name:'السيراميك والأرضيات', checklist:['اعتماد المواد','فحص الاستواء','تجهيز المونة','التركيب','القص','الفواصل','الجراوت','التنظيف','فحص الجودة']},
  {key:'doors', name:'الأبواب والنوافذ والزجاج', checklist:['مراجعة المقاسات','التصنيع','الإطارات','التركيب','الأقفال','المفصلات','الزجاج','السيليكون','الاختبار','الفحص']},
  {key:'kitchen', name:'المطابخ والخزائن الثابتة', checklist:['اعتماد التصميم','مراجعة المقاسات','التصنيع','التركيب','الأسطح','الأجهزة','الإكسسوارات','الفحص']},
  {key:'sanitary', name:'المغاسل والأدوات الصحية', checklist:['تركيب المغاسل','الخلاطات','المراحيض','الدش','المرايا','الخزائن','اختبار التسريب','اختبار التشغيل','الفحص']},
  {key:'handover', name:'التسليم النهائي', checklist:['Punch List','معالجة الملاحظات','اختبار الأنظمة','الكهرباء','السباكة','التكييف','الأبواب','المطابخ','الأدوات الصحية','التنظيف النهائي','As-Built Drawings','مفاتيح المشروع','اعتماد التسليم','إغلاق المشروع']},
];
const FU_EXEC_VERSION = 3;
const FU_TASK_STATUSES = [
  {k:'not_started', ar:'لم يبدأ',     color:'#6b7280'},
  {k:'in_progress', ar:'جاري التنفيذ', color:'#2563eb'},
  {k:'done',        ar:'مكتمل',       color:'#16a34a'},
  {k:'paused',      ar:'متوقف',       color:'#ea580c'},
  {k:'review',      ar:'يحتاج مراجعة', color:'#9333ea'},
  {k:'has_note',    ar:'يوجد ملاحظة',  color:'#d97706'},
];
const FU_PRIORITIES = [
  {k:'low',    ar:'منخفض', color:'#6b7280'},
  {k:'medium', ar:'متوسط', color:'#2563eb'},
  {k:'urgent', ar:'عاجل',  color:'#dc2626'},
];
const FU_NOTE_SEVERITIES = [
  {k:'low',      ar:'منخفض'},
  {k:'medium',   ar:'متوسط'},
  {k:'high',     ar:'عالي'},
  {k:'critical', ar:'حرج'},
];
const FU_NOTE_STATUSES = [
  {k:'open',         ar:'مفتوحة'},
  {k:'in_progress',  ar:'جاري المعالجة'},
  {k:'awaiting',     ar:'بانتظار إعادة الفحص'},
  {k:'closed',       ar:'مغلقة'},
];
const FU_WORKER_STATUSES = ['نشط','متوقف','غائب','منتهي'];
const FU_WORKSHOP_STATUSES = ['نشطة','متوقفة','منتهية'];
// Workshop types — merged from SETTINGS (dynamic) + built-in defaults
const FU_WS_DEFAULTS = ['ورشة حدادة','ورشة نجارة','ورشة بلوك','ورشة لياسة','ورشة دهانات',
  'ورشة كهرباء','ورشة سباكة','ورشة تكييف','ورشة ألمنيوم','ورشة أبواب',
  'ورشة مطابخ','ورشة سيراميك','ورشة خرسانة','أخرى'];
function getWorkshopTypes() {
  const custom = SETTINGS?.workshopTypes || [];
  // Merge: custom first, then defaults not already in custom
  const all = [...custom];
  FU_WS_DEFAULTS.forEach(d => { if(!all.includes(d)) all.push(d); });
  return all;
}
// Keep FU_WORKSHOP_TYPES as getter alias for backwards compat
Object.defineProperty(window, 'FU_WORKSHOP_TYPES', {
  get() { return getWorkshopTypes(); }, configurable: true
});
function fuUID(p){ return (p||'id')+'-'+Date.now().toString(36)+Math.random().toString(36).slice(2,6); }
function fuMigrateTask(c){
  if(c && c.id && c.status && Array.isArray(c.notes)) return c;
  return {
    id: fuUID('t'),
    text: (c && c.text) || 'بند جديد',
    done: !!(c && c.done),
    status: (c && c.done) ? 'done' : 'not_started',
    createdAt: Date.now(), startedAt: null, completedAt: (c && c.done) ? Date.now() : null,
    progress: (c && c.done) ? 100 : 0,
    priority: 'medium',
    assignType: null, assignId: null,
    notes: [],
  };
}
const FU_ISSUE_TYPES = ['تأخر توريد','نقص عمال','مشكلة تصميم','مشكلة موقع','تأخر دفعات العميل','أخرى'];
const FU_ACCEPT = '.pdf,.dwg,.jpg,.jpeg,.png,.docx,.zip';

let FU_CUR = null;      // current project id
let FU_TAB = 'phases';
let FU_EXPANDED = {};   // persistent accordion: stageKey → bool

function fuKindOf(p){
  if(!p) return null;
  if(p.taskTypeKey==='design'||p.taskTypeKey==='permit') return 'design';
  if(p.taskTypeKey==='exec'||p.taskTypeKey==='super') return 'exec';
  return null;
}
function fuEnsure(p){
  if(!p.tracking) p.tracking={};
  const kind=fuKindOf(p);
  if(kind==='design'&&!p.tracking.designPhases){
    p.tracking.designPhases=FU_DESIGN_PHASES.map(ph=>({
      key:ph.key,name:ph.name,progress:0,startDate:'',updatedAt:0,
      engineerId:p.engineerId||null,notes:'',files:[]
    }));
  }
  if(kind==='exec'){
    if(!p.tracking.execStages || p.tracking.execVersion!==FU_EXEC_VERSION){
      const old = p.tracking.execStages || [];
      p.tracking.execStages = FU_EXEC_STAGES.map(st=>{
        const prev = old.find(o=>o.key===st.key);
        return {
          key:st.key, name:st.name,
          progress: prev?.progress ?? 0,
          notes: prev?.notes ?? '',
          checklist: st.checklist.map(t=>{
            const m = prev?.checklist?.find(c=>c.text===t);
            return fuMigrateTask(m || {text:t, done:false});
          }),
          workers: prev?.workers ?? [],
          issues: prev?.issues ?? [],
          files: prev?.files ?? [],
        };
      });
      p.tracking.execVersion = FU_EXEC_VERSION;
    }
    if(!p.tracking.dailyLogs) p.tracking.dailyLogs=[];
  }
  if(!p.workforce) p.workforce = {workers:[], workshops:[]};
  if(!Array.isArray(p.workforce.workers))   p.workforce.workers   = [];
  if(!Array.isArray(p.workforce.workshops)) p.workforce.workshops = [];
  // Migrate workers — add missing fields
  p.workforce.workers.forEach(w => {
    if(w.days    === undefined) w.days    = 0;
    if(!w.payments)             w.payments= [];
  });
  // Migrate workshops — add qty/unit/unitPrice/item/payments
  p.workforce.workshops.forEach(s => {
    if(s.qty       === undefined) s.qty       = 0;
    if(!s.unit)                   s.unit      = 'م²';
    if(s.unitPrice === undefined) s.unitPrice = 0;
    if(!s.item)                   s.item      = '';
    if(!s.payments)               s.payments  = [];
  });
  return p;
}

function openFollowup(id){
  FU_EXPANDED = {};
  const p=STATE.projects.find(x=>x.id===id);
  if(!p){ toast('المشروع غير موجود'); return; }
  const kind=fuKindOf(p);
  if(!kind){
    toast('نظام المتابعة متاح لمشاريع التصميم/الرخص أو التنفيذ/الإشراف فقط');
    return;
  }
  fuEnsure(p);
  FU_CUR=id;
  FU_TAB=(kind==='design')?'phases':'stages';
  const c=STATE.clients.find(cl=>cl.id===p.clientId);
  const t=TYPES[p.taskTypeKey];
  document.getElementById('fu-title').textContent=`متابعة — ${p.projectCode}`;
  document.getElementById('fu-subtitle').innerHTML=`<span class="badge ${t?.badge}">${t?.icon} ${t?.ar}</span> &nbsp; ${esc(c?.name||'')} &nbsp; — &nbsp; ${esc(p.description||'')}`;
  document.getElementById('fu-overlay').classList.add('open');
  fuRender();
}
function closeFollowup(){ document.getElementById('fu-overlay').classList.remove('open'); FU_CUR=null; }

async function fuSave(){
  const p=STATE.projects.find(x=>x.id===FU_CUR);
  if(!p) return;
  p.updatedAt=Date.now();
  await dbPut('projects',p);
}

function fuRender(){
  const p=STATE.projects.find(x=>x.id===FU_CUR);
  if(!p) return;
  const kind=fuKindOf(p);
  const body=document.getElementById('fu-body');
  let tabs='';
  if(kind==='design'){
    tabs=`<div class="fu-tabs">
      <div class="fu-tab ${FU_TAB==='phases'?'active':''}" onclick="FU_TAB='phases';fuRender();">📐 متابعة التصميم</div>
    </div>`;
    body.innerHTML=tabs+fuRenderDesign(p);
  } else {
    tabs=`<div class="fu-tabs">
      <div class="fu-tab ${FU_TAB==='stages'?'active':''}" onclick="FU_TAB='stages';fuRender();">🏗️ مراحل التنفيذ</div>
      <div class="fu-tab ${FU_TAB==='workforce'?'active':''}" onclick="FU_TAB='workforce';fuRender();">👷 العمال والورشات</div>
      <div class="fu-tab ${FU_TAB==='daily'?'active':''}" onclick="FU_TAB='daily';fuRender();">📅 السجل اليومي للموقع</div>
    </div>`;
    let content;
    if(FU_TAB==='daily') content = fuRenderDaily(p);
    else if(FU_TAB==='workforce') content = fuRenderWorkforce(p);
    else content = fuRenderExec(p);
    body.innerHTML = tabs + content;
  }
}

// ─── Engineer options ───
function fuEngOptions(selId){
  return `<option value="">— غير محدد —</option>`+STATE.engineers.map(e=>`<option value="${e.id}" ${String(selId)===String(e.id)?'selected':''}>${esc(e.name)}</option>`).join('');
}

// ═══ DESIGN PHASES ═══
function fuRenderDesign(p){
  return p.tracking.designPhases.map((ph,i)=>{
    const eng=STATE.engineers.find(e=>e.id===ph.engineerId);
    return `<div class="fu-phase" id="fu-ph-${i}">
      <div class="fu-phase-head" onclick="document.getElementById('fu-ph-${i}').classList.toggle('open')">
        <div class="fu-phase-title">
          <span>${i+1}. ${esc(ph.name)}</span>
          <span style="font-size:11px;color:#666;">${eng?'• '+esc(eng.name):''}</span>
        </div>
        <div style="display:flex;align-items:center;gap:10px;">
          <div class="fu-prog"><div class="fu-prog-fill" style="width:${ph.progress||0}%;"></div></div>
          <span style="font-size:12px;font-weight:600;min-width:35px;">${ph.progress||0}%</span>
          <span style="font-size:11px;color:#666;">${ph.files.length} ملف</span>
        </div>
      </div>
      <div class="fu-phase-body">
        <div class="fu-mini">
          <div><label>نسبة الإنجاز %</label><input type="number" min="0" max="100" value="${ph.progress||0}" onchange="fuPhField(${i},'progress',Math.max(0,Math.min(100,parseInt(this.value)||0)))"></div>
          <div><label>تاريخ البدء</label><input type="date" value="${ph.startDate||''}" onchange="fuPhField(${i},'startDate',this.value)"></div>
          <div><label>آخر تحديث</label><input type="text" readonly value="${ph.updatedAt?new Date(ph.updatedAt).toLocaleString('ar-EG'):'—'}"></div>
          <div><label>المهندس المسؤول</label><select onchange="fuPhField(${i},'engineerId',this.value?parseInt(this.value):null)">${fuEngOptions(ph.engineerId)}</select></div>
        </div>
        <div><label style="font-size:11px;color:#666;">ملاحظات وتعليقات</label>
          <textarea rows="2" style="width:100%;padding:6px 8px;border:1px solid #d1d5db;border-radius:6px;font-size:13px;font-family:inherit;" onchange="fuPhField(${i},'notes',this.value)">${esc(ph.notes||'')}</textarea>
        </div>
        <div class="fu-section-title">📎 الملفات وسجل الإصدارات</div>
        <div>
          <label class="fu-btn fu-btn-primary" style="display:inline-flex;">
            <i class="ti ti-upload"></i> رفع ملف جديد
            <input type="file" multiple accept="${FU_ACCEPT}" style="display:none;"
              onchange="fuPhUpload(${i},this)">
          </label>
          <label class="fu-btn-cam" style="display:inline-flex;" title="التقاط صورة من الكاميرا">
            <i class="ti ti-camera"></i> كاميرا
            <input type="file" accept="image/*" capture="environment" style="display:none;"
              onchange="fuPhUpload(${i},this)">
          </label>
          <span style="font-size:11px;color:#666;margin-right:8px;">PDF, DWG, JPG, PNG, DOCX, ZIP</span>
        </div>
        <div style="margin-top:10px;">${fuRenderFiles(ph.files,`fuPhFileAction(${i}`)}</div>
      </div>
    </div>`;
  }).join('');
}
async function fuPhField(i,k,v){
  const p=STATE.projects.find(x=>x.id===FU_CUR);
  p.tracking.designPhases[i][k]=v;
  p.tracking.designPhases[i].updatedAt=Date.now();
  await fuSave();
  if(k==='progress') fuRender();
}
function fuPhUpload(i,inp){ fuUploadInto('designPhases',i,inp); inp.value=''; }
window.fuPhFileAction=function(i,fileId,action,val){ fuFileAction('designPhases',i,fileId,action,val); };

// ═══ EXEC STAGES ═══
function fuCalcStageProgress(stage) {
  const total = (stage.checklist||[]).length;
  if (!total) return stage.progress || 0;
  return Math.round(stage.checklist.filter(c=>c.done).length / total * 100);
}
function fuToggleStage(i, key) {
  FU_EXPANDED[key] = !FU_EXPANDED[key];
  const el  = document.getElementById('fu-st-'+i);
  const ico = document.getElementById('fu-st-ico-'+i);
  if (el)  el.classList.toggle('open', !!FU_EXPANDED[key]);
  if (ico) ico.style.transform = FU_EXPANDED[key] ? 'rotate(180deg)' : '';
}
function fuAssigneeOptions(p, assignType, assignId){
  const wks = (p.workforce?.workers||[]);
  const sps = (p.workforce?.workshops||[]);
  const cur = assignType && assignId ? `${assignType}:${assignId}` : '';
  let html = `<option value="">— غير مكلف —</option>`;
  if(wks.length){
    html += `<optgroup label="👷 العمال">`+wks.map(w=>{
      const v=`worker:${w.id}`;
      return `<option value="${v}" ${cur===v?'selected':''}>${esc(w.name||'بدون اسم')}${w.job?' — '+esc(w.job):''}</option>`;
    }).join('')+`</optgroup>`;
  }
  if(sps.length){
    html += `<optgroup label="🏭 الورشات">`+sps.map(s=>{
      const v=`workshop:${s.id}`;
      return `<option value="${v}" ${cur===v?'selected':''}>${esc(s.name||'بدون اسم')}${s.type?' — '+esc(s.type):''}</option>`;
    }).join('')+`</optgroup>`;
  }
  return html;
}
function fuAssigneeLabel(p, assignType, assignId){
  if(!assignType||!assignId) return '— غير مكلف —';
  if(assignType==='worker'){
    const w=(p.workforce?.workers||[]).find(x=>x.id===assignId);
    return w ? `👷 ${w.name||'عامل'}` : '— محذوف —';
  }
  if(assignType==='workshop'){
    const s=(p.workforce?.workshops||[]).find(x=>x.id===assignId);
    return s ? `🏭 ${s.name||'ورشة'}` : '— محذوفة —';
  }
  return '—';
}
function fuFmtDate(ts){ return ts? new Date(ts).toLocaleDateString('ar-EG') : '—'; }
function fuFmtDT(ts){ return ts? new Date(ts).toLocaleString('ar-EG') : '—'; }

function fuRenderTask(p, i, j, t){
  const stCfg = FU_TASK_STATUSES.find(s=>s.k===t.status) || FU_TASK_STATUSES[0];
  const prCfg = FU_PRIORITIES.find(s=>s.k===t.priority) || FU_PRIORITIES[1];
  const openCls = t._open ? 'open' : '';
  return `<div class="fu-task ${openCls}" style="border:1px solid #e5e7eb;border-radius:8px;padding:8px;margin-bottom:6px;background:#fff;">
    <div style="display:flex;align-items:center;gap:8px;flex-wrap:wrap;">
      <input type="checkbox" ${t.done?'checked':''} onchange="fuTaskDone(${i},${j},this.checked)">
      <input type="text" value="${esc(t.text)}" onchange="fuTaskField(${i},${j},'text',this.value)" style="flex:1;min-width:160px;padding:5px 8px;border:1px solid #d1d5db;border-radius:6px;font-size:13px;">
      <span style="font-size:11px;padding:2px 8px;border-radius:10px;background:${stCfg.color}20;color:${stCfg.color};border:1px solid ${stCfg.color}40;">${stCfg.ar}</span>
      <span style="font-size:11px;padding:2px 8px;border-radius:10px;background:${prCfg.color}20;color:${prCfg.color};border:1px solid ${prCfg.color}40;">⚡ ${prCfg.ar}</span>
      <span style="font-size:11px;color:#666;">${t.progress||0}%</span>
      <span style="font-size:11px;color:#666;">📝 ${(t.notes||[]).length}</span>
      <button class="fu-btn" onclick="fuTaskToggle(${i},${j})" title="تفاصيل"><i class="ti ti-chevron-down"></i> تفاصيل</button>
      <button class="fu-btn fu-btn-danger" onclick="fuTaskDel(${i},${j})"><i class="ti ti-trash"></i> حذف</button>
    </div>
    ${t._open ? `
    <div style="margin-top:8px;padding-top:8px;border-top:1px dashed #e5e7eb;">
      <div class="fu-mini">
        <div><label>الحالة</label><select onchange="fuTaskField(${i},${j},'status',this.value)">
          ${FU_TASK_STATUSES.map(s=>`<option value="${s.k}" ${t.status===s.k?'selected':''}>${s.ar}</option>`).join('')}
        </select></div>
        <div><label>الأولوية</label><select onchange="fuTaskField(${i},${j},'priority',this.value)">
          ${FU_PRIORITIES.map(s=>`<option value="${s.k}" ${t.priority===s.k?'selected':''}>${s.ar}</option>`).join('')}
        </select></div>
        <div><label>نسبة الإنجاز %</label><input type="number" min="0" max="100" value="${t.progress||0}" onchange="fuTaskField(${i},${j},'progress',Math.max(0,Math.min(100,parseInt(this.value)||0)))"></div>
        <div><label>المكلَّف</label><select onchange="fuTaskAssign(${i},${j},this.value)">${fuAssigneeOptions(p, t.assignType, t.assignId)}</select></div>
        <div><label>تاريخ الإنشاء</label><input type="text" readonly value="${fuFmtDT(t.createdAt)}"></div>
        <div><label>تاريخ البدء</label><input type="date" value="${t.startedAt? new Date(t.startedAt).toISOString().slice(0,10):''}" onchange="fuTaskField(${i},${j},'startedAt',this.value? new Date(this.value).getTime():null)"></div>
        <div><label>تاريخ الإنجاز</label><input type="date" value="${t.completedAt? new Date(t.completedAt).toISOString().slice(0,10):''}" onchange="fuTaskField(${i},${j},'completedAt',this.value? new Date(this.value).getTime():null)"></div>
      </div>
      <div class="fu-section-title" style="margin-top:8px;">📝 ملاحظات البند</div>
      <div>${(t.notes||[]).map((n,k)=>fuRenderNote(p,i,j,k,n)).join('') || '<div style="font-size:12px;color:#999;">لا توجد ملاحظات</div>'}</div>
      <button class="fu-btn" onclick="fuNoteAdd(${i},${j})"><i class="ti ti-plus"></i> إضافة ملاحظة</button>
    </div>` : ''}
  </div>`;
}
function fuRenderNote(p,i,j,k,n){
  const photos = (n.photos||[]).map((src,pi)=>`<div style="position:relative;display:inline-block;margin:2px;"><img src="${src}" style="height:60px;border-radius:4px;border:1px solid #ddd;"><button onclick="fuNotePhotoDel(${i},${j},${k},${pi})" style="position:absolute;top:0;left:0;background:rgba(255,0,0,.8);color:#fff;border:none;border-radius:50%;width:16px;height:16px;font-size:10px;cursor:pointer;"> <i class="ti ti-trash" style="font-size:10px;"></i> حذف</button></div>`).join('');
  const files = (n.files||[]).map((f,fi)=>`<div style="display:inline-flex;align-items:center;gap:4px;padding:3px 6px;background:#f3f4f6;border-radius:4px;margin:2px;font-size:11px;"><a href="${f.dataUrl}" download="${esc(f.name)}">📄 ${esc(f.name)}</a><button onclick="fuNoteFileDel(${i},${j},${k},${fi})" style="border:none;background:transparent;color:#dc2626;cursor:pointer;"> <i class="ti ti-trash" style="font-size:10px;"></i> حذف</button></div>`).join('');
  return `<div style="border:1px solid #fde68a;background:#fffbeb;border-radius:6px;padding:6px;margin-bottom:5px;">
    <textarea rows="2" placeholder="نص الملاحظة..." style="width:100%;padding:5px;border:1px solid #d1d5db;border-radius:4px;font-size:12px;font-family:inherit;" onchange="fuNoteField(${i},${j},${k},'text',this.value)">${esc(n.text||'')}</textarea>
    <div class="fu-mini" style="margin-top:5px;">
      <div><label>الكاتب</label><input type="text" value="${esc(n.author||'')}" onchange="fuNoteField(${i},${j},${k},'author',this.value)"></div>
      <div><label>التاريخ</label><input type="text" readonly value="${fuFmtDT(n.date)}"></div>
      <div><label>الخطورة</label><select onchange="fuNoteField(${i},${j},${k},'severity',this.value)">
        ${FU_NOTE_SEVERITIES.map(s=>`<option value="${s.k}" ${n.severity===s.k?'selected':''}>${s.ar}</option>`).join('')}
      </select></div>
      <div><label>الحالة</label><select onchange="fuNoteField(${i},${j},${k},'status',this.value)">
        ${FU_NOTE_STATUSES.map(s=>`<option value="${s.k}" ${n.status===s.k?'selected':''}>${s.ar}</option>`).join('')}
      </select></div>
      <div><label>المسؤول</label><select onchange="fuNoteAssign(${i},${j},${k},this.value)">${fuAssigneeOptions(p, n.assignType, n.assignId)}</select></div>
      <div><label>تاريخ التكليف</label><input type="text" readonly value="${fuFmtDate(n.assignedAt)}"></div>
      <div><label>موعد الحل</label><input type="date" value="${n.dueDate||''}" onchange="fuNoteField(${i},${j},${k},'dueDate',this.value)"></div>
    </div>
    <label style="font-size:11px;color:#666;margin-top:4px;display:block;">رد المسؤول</label>
    <textarea rows="2" style="width:100%;padding:5px;border:1px solid #d1d5db;border-radius:4px;font-size:12px;font-family:inherit;" onchange="fuNoteField(${i},${j},${k},'response',this.value)">${esc(n.response||'')}</textarea>
    <div style="margin-top:5px;">${photos}${files}</div>
    <div style="display:flex;gap:5px;margin-top:5px;justify-content:space-between;">
      <div style="display:flex;gap:5px;">
        <label class="fu-btn" style="font-size:11px;">
          <i class="ti ti-photo"></i> صورة
          <input type="file" multiple accept="image/*" style="display:none;"
            onchange="fuNotePhotoAdd(${i},${j},${k},this)">
        </label>
        <label class="fu-btn-cam" style="font-size:11px;padding:5px 10px;"
          title="كاميرا مباشرة">
          <i class="ti ti-camera"></i> كاميرا
          <input type="file" accept="image/*" capture="environment" style="display:none;"
            onchange="fuNotePhotoAdd(${i},${j},${k},this)">
        </label>
        <label class="fu-btn" style="font-size:11px;"><i class="ti ti-paperclip"></i> ملف<input type="file" multiple accept="${FU_ACCEPT}" style="display:none;" onchange="fuNoteFileAdd(${i},${j},${k},this)"></label>
      </div>
      <button class="fu-btn fu-btn-danger" style="font-size:11px;" onclick="fuNoteDel(${i},${j},${k})"><i class="ti ti-trash"></i> حذف</button>
    </div>
  </div>`;
}
function fuRenderExec(p){
  return p.tracking.execStages.map((st,i)=>{
    const checkDone  = st.checklist.filter(c=>c.done).length;
    const checkTotal = st.checklist.length;
    const notesCount = st.checklist.reduce((a,c)=>a+((c.notes||[]).length),0);
    const autoPct    = fuCalcStageProgress(st);
    if (st.progress !== autoPct) st.progress = autoPct;
    const isOpen   = !!FU_EXPANDED[st.key];
    const openCls  = isOpen ? 'open' : '';
    const chevRot  = isOpen ? 'transform:rotate(180deg);' : '';
    const progColor= autoPct>=100?'#16a34a':autoPct>=50?'#2563eb':'#ea580c';
    return `<div class="fu-phase ${openCls}" id="fu-st-${i}">
      <div class="fu-phase-head" onclick="fuToggleStage(${i},'${st.key}')">
        <div class="fu-phase-title">
          <span>${i+1}. ${esc(st.name)}</span>
          <span style="font-size:11px;color:#666;">
            ✓ ${checkDone}/${checkTotal}
            ${autoPct===100?'<span style="color:#16a34a;font-weight:700;"> ✅ مكتملة</span>':''}
            • 📝 ${notesCount}
          </span>
        </div>
        <div style="display:flex;align-items:center;gap:10px;">
          <div class="fu-prog"><div class="fu-prog-fill" style="width:${autoPct}%;background:${progColor};"></div></div>
          <span style="font-size:12px;font-weight:700;min-width:38px;color:${progColor};">${autoPct}%</span>
          <i class="ti ti-chevron-down" id="fu-st-ico-${i}"
            style="font-size:16px;color:#666;transition:transform .2s;${chevRot}"></i>
        </div>
      </div>
      <div class="fu-phase-body">
        <div style="padding:4px 0 10px;font-size:12px;color:#666;">
          الإنجاز يُحسب تلقائياً:
          <strong style="color:${progColor};">${checkDone}/${checkTotal} بند (${autoPct}%)</strong>
        </div>
        <div class="fu-section-title">✅ Checklist — مهام المرحلة</div>
        <div>${st.checklist.map((c,j)=>fuRenderTask(p,i,j,c)).join('')}</div>
        <button class="fu-btn" onclick="fuClAdd(${i})"><i class="ti ti-plus"></i> إضافة بند</button>

        <div class="fu-section-title">📎 ملاحظات عامة وملفات المرحلة</div>
        <textarea rows="2" style="width:100%;padding:6px 8px;border:1px solid #d1d5db;border-radius:6px;font-size:13px;font-family:inherit;margin-bottom:8px;" placeholder="ملاحظات عامة للمرحلة..." onchange="fuStField(${i},'notes',this.value)">${esc(st.notes||'')}</textarea>
        <div class="cam-wrap">
          <label class="fu-btn fu-btn-primary" style="display:inline-flex;">
            <i class="ti ti-upload"></i> رفع ملف
            <input type="file" multiple accept="${FU_ACCEPT}" style="display:none;"
              onchange="fuStUpload(${i},this)">
          </label>
          <label class="fu-btn-cam" title="التقاط صورة مباشرة من الكاميرا">
            <i class="ti ti-camera"></i> كاميرا
            <input type="file" accept="image/*" capture="environment"
              style="display:none;" onchange="fuStUpload(${i},this)">
          </label>
        </div>
        <div style="margin-top:10px;">${fuRenderFiles(st.files,`fuStFileAction(${i}`)}</div>
      </div>
    </div>`;
  }).join('');
}
async function fuStField(i,k,v){
  const p=STATE.projects.find(x=>x.id===FU_CUR);
  p.tracking.execStages[i][k]=v;
  await fuSave();
  // progress is auto-calculated from checklist — no manual re-render
}
function _fuTask(i,j){ const p=STATE.projects.find(x=>x.id===FU_CUR); return {p, t:p.tracking.execStages[i].checklist[j]}; }
async function fuClAdd(i){
  const p=STATE.projects.find(x=>x.id===FU_CUR);
  const stage=p.tracking.execStages[i];
  stage.checklist.push(fuMigrateTask({text:'بند جديد',done:false}));
  stage.progress=fuCalcStageProgress(stage);
  await fuSave(); fuRender();
}
async function fuTaskDel(i,j){
  if(!confirm('حذف هذا البند؟')) return;
  const p=STATE.projects.find(x=>x.id===FU_CUR);
  const stage=p.tracking.execStages[i];
  stage.checklist.splice(j,1);
  stage.progress=fuCalcStageProgress(stage);
  await fuSave(); fuRender();
}
async function fuTaskToggle(i,j){ const {t}=_fuTask(i,j); t._open=!t._open; fuRender(); }
async function fuTaskDone(i,j,v){
  const p=STATE.projects.find(x=>x.id===FU_CUR);
  const stage=p.tracking.execStages[i];
  const t=stage.checklist[j];
  t.done=v;
  if(v){ t.status='done'; t.progress=100; t.completedAt=Date.now(); }
  else if(t.status==='done'){ t.status='in_progress'; t.completedAt=null; }
  stage.progress=fuCalcStageProgress(stage);
  await fuSave(); fuRender();
}
async function fuTaskField(i,j,k,v){
  const p=STATE.projects.find(x=>x.id===FU_CUR);
  const stage=p.tracking.execStages[i];
  const t=stage.checklist[j];
  t[k]=v;
  if(k==='status'){ t.done=(v==='done'); if(v==='done'){ t.progress=100; t.completedAt=t.completedAt||Date.now(); } if(v==='in_progress'&&!t.startedAt) t.startedAt=Date.now(); }
  if(k==='progress'){ if(v>=100){ t.done=true; t.status='done'; t.completedAt=t.completedAt||Date.now(); } else if(v>0&&t.status==='not_started'){ t.status='in_progress'; t.startedAt=t.startedAt||Date.now(); } }
  stage.progress=fuCalcStageProgress(stage);
  await fuSave(); fuRender();
}
async function fuTaskAssign(i,j,val){
  const {t}=_fuTask(i,j);
  if(!val){ t.assignType=null; t.assignId=null; }
  else{ const [type,id]=val.split(':'); t.assignType=type; t.assignId=id; }
  await fuSave(); fuRender();
}

// Notes per task
async function fuNoteAdd(i,j){ const {t}=_fuTask(i,j); t.notes=t.notes||[]; t.notes.push({id:fuUID('n'),text:'',author:(CU&&CU.name)||'',date:Date.now(),severity:'medium',status:'open',assignType:null,assignId:null,assignedAt:null,dueDate:'',response:'',photos:[],files:[]}); if(t.status==='not_started') t.status='has_note'; await fuSave(); fuRender(); }
async function fuNoteDel(i,j,k){ if(!confirm('حذف الملاحظة؟')) return; const {t}=_fuTask(i,j); t.notes.splice(k,1); await fuSave(); fuRender(); }
async function fuNoteField(i,j,k,key,v){ const {t}=_fuTask(i,j); t.notes[k][key]=v; await fuSave(); }
async function fuNoteAssign(i,j,k,val){ const {t}=_fuTask(i,j); const n=t.notes[k]; if(!val){ n.assignType=null; n.assignId=null; n.assignedAt=null; } else { const [type,id]=val.split(':'); n.assignType=type; n.assignId=id; n.assignedAt=Date.now(); } await fuSave(); fuRender(); }
async function fuNotePhotoAdd(i,j,k,inp){ const {t}=_fuTask(i,j); const n=t.notes[k]; n.photos=n.photos||[]; for(const f of Array.from(inp.files)){ if(f.size>4*1024*1024){ toast('الصورة أكبر من 4MB'); continue; } await new Promise(res=>{const r=new FileReader();r.onload=e=>{n.photos.push(e.target.result);res();};r.readAsDataURL(f);}); } inp.value=''; await fuSave(); fuRender(); }
async function fuNotePhotoDel(i,j,k,pi){ const {t}=_fuTask(i,j); t.notes[k].photos.splice(pi,1); await fuSave(); fuRender(); }
async function fuNoteFileAdd(i,j,k,inp){ const {t}=_fuTask(i,j); const n=t.notes[k]; n.files=n.files||[]; for(const f of Array.from(inp.files)){ if(f.size>4*1024*1024){ toast('الملف أكبر من 4MB'); continue; } const dataUrl=await new Promise(res=>{const r=new FileReader();r.onload=e=>res(e.target.result);r.readAsDataURL(f);}); n.files.push({id:fuUID('f'),name:f.name,size:f.size,type:f.type,dataUrl}); } inp.value=''; await fuSave(); fuRender(); }
async function fuNoteFileDel(i,j,k,fi){ const {t}=_fuTask(i,j); t.notes[k].files.splice(fi,1); await fuSave(); fuRender(); }

function fuStUpload(i,inp){ fuUploadInto('execStages',i,inp); inp.value=''; }
window.fuStFileAction=function(i,fileId,action,val){ fuFileAction('execStages',i,fileId,action,val); };

// ═══ WORKFORCE (workers + workshops) ═══
function fuRenderWorkforce(p){
  const wks = p.workforce.workers  || [];
  const sps = p.workforce.workshops || [];
  const fin = getProjFin(p);
  const cur = fin.currency || p.currency || 'USD';

  // ── Workers table ───────────────────────────────────────────────
  const wkRows = wks.map(w=>{
    if(!w.payments) w.payments=[];
    const total   = wkTotal(w);
    const paid    = wkPaid(w);
    const rem     = total - paid;
    const payChips= w.payments.map(pm=>`<span class="wf-pay-chip">${fmt(pm.amount||0,cur)}</span>`).join('');
    return `<tr>
      <td><input class="wf-inp" value="${esc(w.name||'')}" placeholder="الاسم" onchange="fuWkField('${w.id}','name',this.value)"></td>
      <td><input class="wf-inp" value="${esc(w.job||'')}" placeholder="المهنة" onchange="fuWkField('${w.id}','job',this.value)"></td>
      <td><input class="wf-inp" value="${esc(w.phone||'')}" placeholder="الهاتف" onchange="fuWkField('${w.id}','phone',this.value)"></td>
      <td class="td-num"><input type="number" min="0" value="${w.dailyWage||''}" placeholder="0"
        onchange="fuWkField('${w.id}','dailyWage',parseFloat(this.value)||0)"></td>
      <td class="td-num"><input type="number" min="0" value="${w.days||''}" placeholder="0"
        onchange="fuWkField('${w.id}','days',parseFloat(this.value)||0)"></td>
      <td class="td-calc">${fmt(total,cur)}</td>
      <td class="td-paid">${fmt(paid,cur)}<br><small style="font-weight:400;color:#6b7280;">${payChips}</small></td>
      <td class="td-rem" style="color:${rem>0?'var(--red)':'var(--green)'};">${rem>0?fmt(rem,cur):'✓'}</td>
      <td><select onchange="fuWkField('${w.id}','status',this.value)">${FU_WORKER_STATUSES.map(s=>`<option ${w.status===s?'selected':''}>${s}</option>`).join('')}</select></td>
      <td style="text-align:center;white-space:nowrap;">
        <button class="wf-pay-btn" onclick="fuWkPayOpen('${w.id}')"><i class="ti ti-cash"></i> دفعة</button>
      </td>
      <td style="text-align:center;">
        <button class="fu-btn fu-btn-danger" onclick="fuWkDel('${w.id}')"><i class="ti ti-trash"></i> حذف</button>
      </td>
    </tr>`;
  }).join('') || `<tr><td colspan="11" style="text-align:center;padding:15px;color:#999;">لا يوجد عمال</td></tr>`;

  const wkTotalAll = wks.reduce((s,w)=>s+wkTotal(w),0);
  const wkPaidAll  = wks.reduce((s,w)=>s+wkPaid(w),0);

  // ── Workshops table ─────────────────────────────────────────────
  const spRows = sps.map(s=>{
    if(!s.payments) s.payments=[];
    const total    = spTotal(s);
    const paid     = spPaid(s);
    const rem      = total - paid;
    const payChips = s.payments.map(pm=>{
      const typeLbl = {advance:'مقدمة',milestone:'مرحلية',final:'نهائية'}[pm.type]||pm.type||'دفعة';
      return `<span class="wf-pay-chip">${typeLbl}: ${fmt(pm.amount||0,cur)}</span>`;
    }).join('');
    return `<tr>
      <td><input class="wf-inp" value="${esc(s.name||'')}" placeholder="اسم الورشة" onchange="fuSpField('${s.id}','name',this.value)"></td>
      <td><input class="wf-inp" value="${esc(s.manager||'')}" placeholder="المسؤول" onchange="fuSpField('${s.id}','manager',this.value)"></td>
      <td><input class="wf-inp" value="${esc(s.phone||'')}" placeholder="الهاتف" onchange="fuSpField('${s.id}','phone',this.value)"></td>
      <td><select onchange="fuSpTypeChange('${s.id}',this)">
        ${getWorkshopTypes().map(t=>`<option ${s.type===t?'selected':''}>${esc(t)}</option>`).join('')}
        <option value="__new__" style="color:var(--accent);font-weight:700;">＋ إضافة نوع جديد...</option>
      </select></td>
      <td><input class="wf-inp" value="${esc(s.item||'')}" placeholder="البند / المرحلة" onchange="fuSpField('${s.id}','item',this.value)"></td>
      <td class="td-num"><input type="number" min="0" value="${s.qty||''}" placeholder="0"
        onchange="fuSpField('${s.id}','qty',parseFloat(this.value)||0)"></td>
      <td><input class="wf-inp" value="${esc(s.unit||'م²')}" placeholder="الوحدة" style="width:60px;" onchange="fuSpField('${s.id}','unit',this.value)"></td>
      <td class="td-num"><input type="number" min="0" value="${s.unitPrice||''}" placeholder="0"
        onchange="fuSpField('${s.id}','unitPrice',parseFloat(this.value)||0)"></td>
      <td class="td-calc">${fmt(total,cur)}</td>
      <td class="td-paid">${fmt(paid,cur)}<br><small style="font-weight:400;color:#6b7280;">${payChips}</small></td>
      <td class="td-rem" style="color:${rem>0?'var(--red)':'var(--green)'};">${rem>0?fmt(rem,cur):'✓'}</td>
      <td><select onchange="fuSpField('${s.id}','status',this.value)">${FU_WORKSHOP_STATUSES.map(st=>`<option ${s.status===st?'selected':''}>${st}</option>`).join('')}</select></td>
      <td style="text-align:center;white-space:nowrap;">
        <button class="wf-pay-btn" onclick="fuSpPayOpen('${s.id}')"><i class="ti ti-cash"></i> دفعة</button>
      </td>
      <td style="text-align:center;">
        <button class="fu-btn fu-btn-danger" onclick="fuSpDel('${s.id}')"><i class="ti ti-trash"></i> حذف</button>
      </td>
    </tr>`;
  }).join('') || `<tr><td colspan="14" style="text-align:center;padding:15px;color:#999;">لا توجد ورشات</td></tr>`;

  const spTotalAll = sps.reduce((s,sp)=>s+spTotal(sp),0);
  const spPaidAll  = sps.reduce((s,sp)=>s+spPaid(sp),0);

  return `
    <!-- Workers -->
    <div class="fu-section-title">👷 العمال المباشرون (${wks.length})
      <span style="font-size:11px;font-weight:400;color:#6b7280;margin-right:8px;">
        إجمالي: ${fmt(wkTotalAll,cur)} | مدفوع: ${fmt(wkPaidAll,cur)} | متبقي: ${fmt(wkTotalAll-wkPaidAll,cur)}
      </span>
    </div>
    <div class="wf-table-wrap">
      <table class="wf-table">
        <thead><tr>
          <th style="min-width:120px;">الاسم</th>
          <th style="min-width:100px;">المهنة</th>
          <th style="min-width:110px;">الهاتف</th>
          <th style="min-width:90px;">أجر يومي</th>
          <th style="min-width:80px;">الأيام</th>
          <th style="min-width:100px;">الإجمالي</th>
          <th style="min-width:110px;">المدفوع</th>
          <th style="min-width:90px;">المتبقي</th>
          <th style="min-width:100px;">الحالة</th>
          <th style="min-width:80px;">دفعة</th>
          <th></th>
        </tr></thead>
        <tbody>${wkRows}</tbody>
      </table>
    </div>
    <button class="fu-btn fu-btn-primary" style="margin-top:8px;" onclick="fuWkAdd()">
      <i class="ti ti-plus"></i> إضافة عامل
    </button>

    <!-- Workshops -->
    <div class="fu-section-title" style="margin-top:18px;">🏭 الورشات / المقاولون الفرعيون (${sps.length})
      <span style="font-size:11px;font-weight:400;color:#6b7280;margin-right:8px;">
        إجمالي: ${fmt(spTotalAll,cur)} | مدفوع: ${fmt(spPaidAll,cur)} | متبقي: ${fmt(spTotalAll-spPaidAll,cur)}
      </span>
    </div>
    <div class="wf-table-wrap">
      <table class="wf-table">
        <thead><tr>
          <th style="min-width:130px;">اسم الورشة</th>
          <th style="min-width:110px;">المسؤول</th>
          <th style="min-width:110px;">الهاتف</th>
          <th style="min-width:130px;">نوع العمل</th>
          <th style="min-width:140px;">البند / المرحلة</th>
          <th style="min-width:80px;">الكمية</th>
          <th style="min-width:70px;">الوحدة</th>
          <th style="min-width:90px;">سعر الوحدة</th>
          <th style="min-width:110px;">قيمة العقد</th>
          <th style="min-width:130px;">المدفوع</th>
          <th style="min-width:90px;">المتبقي</th>
          <th style="min-width:90px;">الحالة</th>
          <th style="min-width:80px;">دفعة</th>
          <th></th>
        </tr></thead>
        <tbody>${spRows}</tbody>
      </table>
    </div>
    <button class="fu-btn fu-btn-primary" style="margin-top:8px;" onclick="fuSpAdd()">
      <i class="ti ti-plus"></i> إضافة ورشة
    </button>

    <style>
      .wf-inp { width:100%; border:none; padding:6px 8px; background:transparent;
                font-size:12.5px; font-family:inherit; box-sizing:border-box; }
      .wf-inp:focus { outline:2px solid var(--accent); background:#fff; border-radius:3px; }
    </style>
  `;
}
async function fuWkAdd(){
  const p=STATE.projects.find(x=>x.id===FU_CUR);
  p.workforce.workers.push({
    id:fuUID('w'), name:'', phone:'', specialty:'', job:'',
    dailyWage:0, monthlyWage:0, days:0, idNumber:'',
    startDate:'', status:'نشط', notes:'', payments:[]
  });
  await fuSave(); fuRender(); wfSyncFinance();
}
async function fuWkDel(id){
  if(!confirm('حذف العامل؟')) return;
  const p=STATE.projects.find(x=>x.id===FU_CUR);
  p.workforce.workers=p.workforce.workers.filter(w=>w.id!==id);
  await fuSave(); fuRender(); wfSyncFinance();
}
async function fuWkField(id,k,v){
  const p=STATE.projects.find(x=>x.id===FU_CUR);
  const w=p.workforce.workers.find(x=>x.id===id); if(!w) return;
  if(!w.payments) w.payments=[];  // migrate
  w[k]=v; await fuSave();
  if(['dailyWage','days'].includes(k)) { fuRender(); wfSyncFinance(); }
}
async function fuSpAdd(){
  const p=STATE.projects.find(x=>x.id===FU_CUR);
  p.workforce.workshops.push({
    id:fuUID('s'), name:'', type:getWorkshopTypes()[0]||'ورشة',
    manager:'', phone:'', item:'',
    qty:0, unit:'م²', unitPrice:0, contractValue:0,
    paymentMethod:'', progress:0,
    startDate:'', endDate:'', status:'نشطة', payments:[]
  });
  await fuSave(); fuRender(); wfSyncFinance();
}
async function fuSpDel(id){
  if(!confirm('حذف الورشة؟')) return;
  const p=STATE.projects.find(x=>x.id===FU_CUR);
  p.workforce.workshops=p.workforce.workshops.filter(s=>s.id!==id);
  await fuSave(); fuRender(); wfSyncFinance();
}
async function fuSpField(id,k,v){
  const p=STATE.projects.find(x=>x.id===FU_CUR);
  const s=p.workforce.workshops.find(x=>x.id===id); if(!s) return;
  if(!s.payments) s.payments=[];  // migrate
  s[k]=v; await fuSave();
  if(['qty','unitPrice','contractValue'].includes(k)) { fuRender(); wfSyncFinance(); }
}

// ═══ FILES + VERSIONS ═══
function fuRenderFiles(files,actionPrefix){
  if(!files.length) return '<div style="font-size:12px;color:#999;">لا توجد ملفات</div>';
  // group by baseName
  const groups={};
  files.forEach(f=>{ (groups[f.baseName]=groups[f.baseName]||[]).push(f); });
  return Object.keys(groups).map(bn=>{
    const list=groups[bn].slice().sort((a,b)=>b.version-a.version);
    return `<div style="border:1px solid #e5e7eb;border-radius:6px;padding:8px;margin-bottom:6px;background:#fafbfc;">
      <div style="font-weight:600;font-size:12px;margin-bottom:6px;">📄 ${esc(bn)}</div>
      ${list.map(f=>{
        const stCls=f.status==='approved'?'fu-v-approved':(f.status==='revise'?'fu-v-revise':'fu-v-pending');
        const stTxt=f.status==='approved'?'معتمدة':(f.status==='revise'?'مطلوب تعديل':'بانتظار مراجعة');
        const dl=f.dataUrl?`<a class="fu-btn" href="${f.dataUrl}" download="${esc(f.name)}"><i class="ti ti-download"></i></a>`:'';
        return `<div class="fu-file-item">
          <div style="flex:1;">
            <strong>v${f.version}</strong> &nbsp; ${esc(f.name)}
            <div class="fu-file-meta">${esc(f.uploadedBy||'—')} • ${new Date(f.uploadedAt).toLocaleString('ar-EG')} • ${(f.size/1024).toFixed(1)} KB</div>
            <input type="text" placeholder="ملاحظات النسخة" value="${esc(f.notes||'')}" onchange="${actionPrefix},'${f.id}','notes',this.value)" style="width:100%;margin-top:4px;padding:3px 5px;border:1px solid #d1d5db;border-radius:4px;font-size:11px;">
          </div>
          <div style="display:flex;flex-direction:column;gap:4px;align-items:flex-end;">
            <span class="fu-vbadge ${stCls}">${stTxt}</span>
            <select onchange="${actionPrefix},'${f.id}','status',this.value)" style="font-size:11px;padding:2px;">
              <option value="pending" ${f.status==='pending'?'selected':''}>بانتظار</option>
              <option value="approved" ${f.status==='approved'?'selected':''}>معتمدة</option>
              <option value="revise" ${f.status==='revise'?'selected':''}>تعديل</option>
            </select>
            <div style="display:flex;gap:3px;">${dl}<button class="fu-btn fu-btn-danger" onclick="${actionPrefix},'${f.id}','delete')"><i class="ti ti-trash"></i> حذف</button></div>
          </div>
        </div>`;
      }).join('')}
    </div>`;
  }).join('');
}
async function fuUploadInto(coll,i,inp){
  const p=STATE.projects.find(x=>x.id===FU_CUR);
  const target=p.tracking[coll][i];
  const MAX=4*1024*1024;
  const files=Array.from(inp.files);
  for(const file of files){
    const baseName=file.name.replace(/\s+v\d+(\.[^.]+)?$/i,'').replace(/(\.[^.]+)$/,'');
    const existing=target.files.filter(f=>f.baseName===baseName);
    const version=existing.length?Math.max(...existing.map(f=>f.version))+1:1;
    const entry={id:Date.now()+'-'+Math.random().toString(36).slice(2,7),name:file.name,baseName,size:file.size,type:file.type,version,uploadedBy:(CU&&CU.name)||'مستخدم',uploadedAt:Date.now(),notes:'',status:'pending',dataUrl:null};
    if(file.size<=MAX){
      await new Promise(res=>{const r=new FileReader();r.onload=e=>{entry.dataUrl=e.target.result;res();};r.readAsDataURL(file);});
    }
    target.files.push(entry);
  }
  await fuSave(); fuRender();
}
async function fuFileAction(coll,i,fileId,action,val){
  const p=STATE.projects.find(x=>x.id===FU_CUR);
  const arr=p.tracking[coll][i].files;
  const idx=arr.findIndex(f=>f.id===fileId);
  if(idx<0) return;
  if(action==='delete'){ if(!confirm('حذف هذه النسخة؟')) return; arr.splice(idx,1); }
  else { arr[idx][action]=val; }
  await fuSave(); fuRender();
}

// ═══ DAILY SITE LOG ═══
function fuRenderDaily(p){
  const logs=(p.tracking.dailyLogs||[]).slice().sort((a,b)=>(b.date||'').localeCompare(a.date||''));
  return `<button class="fu-btn fu-btn-primary" onclick="fuLogAdd()"><i class="ti ti-plus"></i> إضافة سجل يومي</button>
    <div style="margin-top:12px;">${logs.length?logs.map(L=>fuRenderLog(L)).join(''):'<div style="text-align:center;color:#999;padding:30px;">لا توجد سجلات يومية</div>'}</div>`;
}
function fuRenderLog(L){
  // Migrate missing fields
  if(!L.issues)     L.issues=[];
  if(!L.summary)    L.summary='';
  if(!L.workshop)   L.workshop='';
  if(!L.status)     L.status='draft';
  const submitted  = L.status==='submitted';
  const readonly   = submitted ? 'readonly disabled' : '';

  // Migrate and render photos with comment threads
  const migratedPhotos = (L.photos||[]).map(migratePhoto);
  const photos = migratedPhotos.map((ph,i)=>renderPhotoCard(ph, L.id, i)).join('');

  // Issues HTML
  const issueRows = (L.issues||[]).map((iss,idx)=>{
    const priClass = iss.priority==='عالية'?'pri-high':iss.priority==='منخفضة'?'pri-low':'';
    return `<div class="log-issue-card ${priClass}">
      <div style="display:flex;align-items:flex-start;gap:8px;flex-wrap:wrap;">
        <div style="flex:1;min-width:150px;">
          <input class="fu-inp" value="${esc(iss.description||'')}" placeholder="وصف المشكلة..."
            onchange="fuLogIssueField('${L.id}',${idx},'description',this.value)"
            style="width:100%;font-weight:600;" ${readonly}>
        </div>
        <div style="display:flex;gap:6px;flex-wrap:wrap;">
          <select onchange="fuLogIssueField('${L.id}',${idx},'workshop',this.value)" ${readonly}
            style="font-size:11.5px;padding:4px 6px;border:1px solid var(--border);border-radius:4px;font-family:inherit;">
            <option value="">الورشة المسؤولة</option>
            ${fuLogGetWorkshops().map(w=>`<option ${iss.workshop===w?'selected':''}>${esc(w)}</option>`).join('')}
          </select>
          <select onchange="fuLogIssueField('${L.id}',${idx},'priority',this.value)" ${readonly}
            style="font-size:11.5px;padding:4px 6px;border:1px solid var(--border);border-radius:4px;font-family:inherit;">
            ${['عالية','متوسطة','منخفضة'].map(pr=>`<option ${iss.priority===pr?'selected':''}>${pr}</option>`).join('')}
          </select>
          <select onchange="fuLogIssueField('${L.id}',${idx},'status',this.value)" ${readonly}
            style="font-size:11.5px;padding:4px 6px;border:1px solid var(--border);border-radius:4px;font-family:inherit;">
            ${['مفتوحة','جاري المعالجة','بانتظار المراجعة','تم الحل','مغلقة'].map(st=>`<option ${iss.status===st?'selected':''}>${st}</option>`).join('')}
          </select>
          <input type="date" value="${iss.resolveBy||''}" title="موعد المعالجة"
            onchange="fuLogIssueField('${L.id}',${idx},'resolveBy',this.value)" ${readonly}
            style="font-size:11px;padding:4px 6px;border:1px solid var(--border);border-radius:4px;">
          ${submitted?'':`<button class="icon-btn del" onclick="fuLogIssueDel('${L.id}',${idx})"><i class="ti ti-trash" style="font-size:12px;"></i> حذف</button>`}
        </div>
      </div>
    </div>`;
  }).join('');
  return `<div class="fu-log" id="log-${L.id}">
    <div style="display:flex;align-items:center;justify-content:space-between;margin-bottom:8px;">
      <span class="log-status-badge ${submitted?'log-status-submitted':'log-status-draft'}">
        ${submitted?'✅ مُرسَل':'📝 مسودة'}
        ${submitted?` — ${L.submittedBy||''} — ${new Date(L.submittedAt||0).toLocaleString('ar-SA')}`:''}
      </span>
      ${!submitted?`<button class="icon-btn del" onclick="fuLogDel('${L.id}')" style="display:flex;align-items:center;gap:4px;padding:5px 10px;border-radius:6px;"><i class="ti ti-trash"></i> حذف السجل</button>`:''}
    </div>
    <div class="fu-mini">
      <div><label>التاريخ</label><input type="date" value="${L.date||''}" onchange="fuLogField('${L.id}','date',this.value)"></div>
      <div><label>عدد العمال</label><input type="number" value="${L.workersCount||0}" onchange="fuLogField('${L.id}','workersCount',parseInt(this.value)||0)"></div>
    </div>
    <label style="font-size:11px;color:#666;">الأعمال المنفذة اليوم</label>
    <textarea rows="2" style="width:100%;padding:6px 8px;border:1px solid #d1d5db;border-radius:6px;font-size:13px;font-family:inherit;margin-bottom:6px;" onchange="fuLogField('${L.id}','work',this.value)">${esc(L.work||'')}</textarea>
    <label style="font-size:11px;color:#666;">المواد المستلمة</label>
    <textarea rows="2" style="width:100%;padding:6px 8px;border:1px solid #d1d5db;border-radius:6px;font-size:13px;font-family:inherit;margin-bottom:6px;" onchange="fuLogField('${L.id}','materials',this.value)">${esc(L.materials||'')}</textarea>
    <label style="font-size:11px;color:#666;">الحوادث (إن وجدت)</label>
    <textarea rows="2" style="width:100%;padding:6px 8px;border:1px solid #d1d5db;border-radius:6px;font-size:13px;font-family:inherit;margin-bottom:6px;" onchange="fuLogField('${L.id}','incidents',this.value)">${esc(L.incidents||'')}</textarea>
    <label style="font-size:11px;color:#666;">ملاحظات</label>
    <textarea rows="2" style="width:100%;padding:6px 8px;border:1px solid #d1d5db;border-radius:6px;font-size:13px;font-family:inherit;margin-bottom:6px;" onchange="fuLogField('${L.id}','notes',this.value)">${esc(L.notes||'')}</textarea>
    <div>${photos}</div>
    <div style="display:flex;justify-content:space-between;margin-top:8px;">
      <div class="cam-wrap">
        <label class="fu-btn"><i class="ti ti-photo"></i> اختيار صور
          <input type="file" multiple accept="image/*" style="display:none;"
            onchange="fuLogPhotoAdd('${L.id}',this)">
        </label>
        <label class="fu-btn-cam" title="التقاط صورة مباشرة من الكاميرا">
          <i class="ti ti-camera"></i> كاميرا
          <input type="file" accept="image/*" capture="environment"
            style="display:none;" onchange="fuLogPhotoAdd('${L.id}',this)">
        </label>
      </div>
      <button class="fu-btn fu-btn-danger" onclick="fuLogDel('${L.id}')"><i class="ti ti-trash"></i> حذف</button>
    </div>
  </div>`;
}
async function fuLogAdd(){
  const p=STATE.projects.find(x=>x.id===FU_CUR);
  p.tracking.dailyLogs.push({
    id:'L'+Date.now(),
    date: new Date().toISOString().slice(0,10),
    work:'', workersCount:0, materials:'',
    photos:[], notes:'', incidents:'',
    summary:'', workshop:'', issues:[],
    status:'draft', submittedAt:null, submittedBy:''
  });
  await fuSave(); fuRender();
}
async function fuLogDel(id){ if(!confirm('حذف السجل؟')) return; const p=STATE.projects.find(x=>x.id===FU_CUR); p.tracking.dailyLogs=p.tracking.dailyLogs.filter(L=>L.id!==id); await fuSave(); fuRender(); }
async function fuLogField(id,k,v){ const p=STATE.projects.find(x=>x.id===FU_CUR); const L=p.tracking.dailyLogs.find(l=>l.id===id); if(!L) return; L[k]=v; await fuSave(); }
async function fuLogPhotoAdd(id, inp) {
  const p = STATE.projects.find(x=>x.id===FU_CUR);
  const L = (p?.tracking?.dailyLogs||[]).find(l=>l.id===id);
  if(!L) return;
  L.photos = (L.photos||[]).map(migratePhoto); // migrate old format
  for(const file of Array.from(inp.files)) {
    if(file.size > 5*1024*1024) { toast('⚠ الصورة أكبر من 5MB'); continue; }
    await new Promise(res => {
      const r = new FileReader();
      r.onload = e => {
        const photoObj = {
          id:         'ph_'+Date.now()+'_'+Math.random().toString(36).slice(2,6),
          src:        e.target.result,
          caption:    '',
          uploadedBy: CU?.name || 'مجهول',
          uploadedAt: Date.now(),
          comments:   [],
        };
        L.photos.push(photoObj);
        res();
      };
      r.readAsDataURL(file);
    });
  }
  await fuSave();
  fuRender();
  toast('✓ تم رفع الصور');
  inp.value = '';
}
async function fuLogPhotoDel(id, i) {
  if(!confirm('حذف هذه الصورة مع جميع تعليقاتها؟')) return;
  const p = STATE.projects.find(x=>x.id===FU_CUR);
  const L = (p?.tracking?.dailyLogs||[]).find(l=>l.id===id); if(!L) return;
  L.photos.splice(i,1);
  await fuSave(); fuRender();
}
</script>



<script>
// ── Startup: check session then show login or app ──
(async function startApp() {
  await initDB();
  // Load dynamic users first
  try {
    const uSaved = localStorage.getItem('pxid_users');
    DUSERS = uSaved ? JSON.parse(uSaved) : null;
  } catch(e) { DUSERS = null; }

  const restored = tryRestoreSession();
  if (restored) {
    // Valid session — go straight to app
    await loadAllData();
    document.getElementById('login-wrap').style.display = 'none';
    document.getElementById('app').style.display = 'flex';
    applyRoleUI();
    renderAll();
  } else {
    // No session — show login
    document.getElementById('login-wrap').style.display = 'flex';
    document.getElementById('app').style.display = 'none';
  }
})();
</script>
</body></html>
