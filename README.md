# PatchGuard-Win11
This repository contains some information for PatchGuard for Windows 11 (build 22000.xxx), to potentially help researchers, security professionals, and enthusiasts looking into PatchGuard for Windows 11.

<h2>KiFilterFiberContext/PatchGuardTVCallback.h</h2>
<p>This header file contains the decompiled notification callback function (a PatchGuard check routine) found at the entry of 'KiFilterFiberContext' if 'PsIntegrityCheckEnabled' is greater than zero. <br>
'ExCreateCallback' opens an existing callback object 'TV' which is registered at boot-time by an external binary.
It is similar to the historical and well-known huge 'FsRtlMdlReadCompleteDevEx'.</p>
<img src="https://i.imgur.com/ypKeYLd.png" alt="TVCallbackRegister">
