---
title: "Telephony advisor for Exchange 2013"
ms.author: tonysmit
author: tonysmit
manager: scotv
ms.date: 6/24/2018
ms.audience: ITPro
ms.topic: article
ms.service: exchange-online
localization_priority: Normal
ms.assetid: e9f760f2-5901-4ed2-95a5-724555cc700e

description: "Unified Messaging (UM) requires that you integrate Microsoft Exchange with the existing telephony system for your organization. A successful deployment requires you to make a careful analysis of your existing telephony infrastructure and to perform the correct planning steps to deploy Unified Messaging."
---

# Telephony advisor for Exchange 2013

Unified Messaging (UM) requires that you integrate Microsoft Exchange with the existing telephony system for your organization. A successful deployment requires you to make a careful analysis of your existing telephony infrastructure and to perform the correct planning steps to deploy Unified Messaging. 
  
The planning phase can be a significant challenge to Exchange administrators who have little or no experience with a telephony network. To help address this challenge, see the following section **Resources to help with your UM deployment**.
  
The other sections in this topic cover the supported VoIP gateways for Unified Messaging, how to determine whether your PBX is supported using a specific VoIP gateway model or manufacturer, whether your IP PBX is supported using a direct SIP connection, and supported session border controllers (SBCs) for Exchange Online UM.
  
## Resources to help with your UM deployment
<a name="resources"> </a>

It's challenging to create guidelines for deploying telephony networks. They can be very different from one another because they can include VoIP gateways, IP PBXs, and PBXs with different configuration settings, firmware, and requirements. However, several resources are available to help you successfully deploy Unified Messaging: 
  
- **Unified Messaging specialists ** UM specialists are systems integrators who have received technical training about Exchange Unified Messaging conducted by the Exchange engineering team. To help ensure a smooth transition to Unified Messaging from legacy voice mail systems, Microsoft recommends that all customers engage a UM specialist. For contact information, visit [Microsoft Exchange Server 2013 Unified Messaging (UM) Specialists](http://go.microsoft.com/fwlink/p/?LinkId=262708) or [Microsoft Pinpoint for Unified Messaging](https://go.microsoft.com/fwlink/p/?LinkId=261951).
    
- **Configuration Notes for Supported VoIP Gateways, IP PBXs and PBXs** These configuration notes contain settings and other information that's very useful when you're configuring VoIP gateways, IP PBXs, and PBXs to communicate with the Unified Messaging servers that are on your network. For more information, see [Configuration notes for supported VoIP gateways, IP PBXs, and PBXs](configuration-notes-for-voip-gateways.md).
    
- **Configuration Notes for Supported Session Border Controllers** These configuration notes contain settings and other information that's very useful when you're configuring session border controllers (SBCs) to communicate with the Unified Messaging servers in hybrid and Exchange Online UM deployments. For more information, see [Configuration notes for supported session border controllers](configuration-notes-for-session-border-controllers.md).
    
    > [!NOTE]
    > Exchange Online UM support for third-party PBX systems via direct connections from customer operated SBCs will end in July 2018. Please see the Exchange team blog [Discontinuation of support for session border controllers in Exchange Online unified messaging](https://blogs.technet.microsoft.com/exchange/2017/07/18/discontinuation-of-support-for-session-border-controllers-in-exchange-online-unified-messaging/) for more information. 
  
Before you engage a Unified Messaging specialist, you should be able to answer key questions that they'll ask. Having the answers to the following questions will help make the conversation between you and the UM specialist productive:
  
- How many existing telephone or voice mail users, or both, are in your organization? 
    
- How many users do you intend to provide with Unified Messaging?
    
- Which PBX or PBXs do you intend to use for integration with Unified Messaging?
    
- How many PBXs does your organization have? Specify the vendors, types (circuit- or IP-based), models, and firmware versions.
    
- Are the PBXs networked, and are they centralized or located in multiple locations?
    
- What voice mail system or systems does your organization currently use? Specify the vendors, types, models, and firmware versions.
    
- How are the voice mail systems integrated into your PBXs (Analog, T1/E1, PRI, Digital set emulation, VoIP, other)?
    
- Are you currently using voice networking?
    
- What type of fax system or systems does your organization use, and does the fax system or systems support inbound fax routing to Exchange?
    
- Does your organization use automated attendants?
    
- Do you need support for phone-only users, that is, users who won't have email access?
    
## Supported VoIP gateways
<a name="supIPgate"> </a>

Integrating Unified Messaging with PBXs requires you to use one or more VoIP gateways to translate the circuit-switched protocols that are used by TDM-based PBXs to IP-based, packet-switched protocols that are used by Unified Messaging. VoIP gateway vendors with several models of VoIP and media gateways have been tested and are supported for Unified Messaging. 
  
Interoperability testing of Unified Messaging with VoIP gateways, IP PBXs, and SBCs is now integrated with the Microsoft Unified Communications Open Interoperability Program. For more information, see [Microsoft Unified Communications Open Interoperability Program](http://go.microsoft.com/fwlink/p/?linkId=140722). 
  
The [Microsoft Unified Communications Open Interoperability Program](http://go.microsoft.com/fwlink/p/?linkId=140722) qualification program for VoIP gateways, IP PBXs, and advanced VoIP gateways ensures that customers have a seamless setup and support experience when they're using qualified telephony VoIP gateways and IP PBXs with Microsoft Unified Communications software. Only products that meet rigorous and extensive testing requirements and conform to the specifications and test plans receive qualification. 
  
For details about configuring supported VoIP gateways, IP PBXs, PBXs, and SBCs, see one of the following resources: 
  
- [Configuration notes for supported VoIP gateways, IP PBXs, and PBXs](configuration-notes-for-voip-gateways.md)
    
- [Configuration notes for supported session border controllers](configuration-notes-for-session-border-controllers.md)
    
Interoperability was verified for the following VoIP gateway vendors:
  
- AudioCodes
    
- Dialogic
    
- The following table shows the VoIP gateway vendor, the VoIP gateway model, and the protocols that are supported by each model.
    
**Supported VoIP gateways for Unified Messaging**

|**Vendor**|**Model**|**Supported protocols**|
|:-----|:-----|:-----|
|AudioCodes  <br/> |MediaPack 114/8 FXO  <br/> | Analog with In-Band DTMF  <br/>  Analog with SMDI  <br/> |
|AudioCodes  <br/> |Mediant 1000  <br/> | Analog with In-Band DTMF  <br/>  Analog with SMDI  <br/>  BRI Q.SIG  <br/>  T1/E1 Q.SIG  <br/>  IP-to-IP  <br/> |
|AudioCodes  <br/> |Mediant 2000  <br/> | T1/E1 CAS  <br/>  T1/E1 Q.SIG  <br/>  IP-to-IP  <br/> |
|Dialogic  <br/> |DMG1000PBXDNIW  <br/> |Digital Set Emulation  <br/> |
|Dialogic  <br/> |DMG1000LSW  <br/> | Analog with In-Band DTMF  <br/>  Analog with SMDI  <br/> |
|Dialogic  <br/> |DMG2000  <br/> | T1 CAS  <br/>  T1/E1 Q.SIG  <br/> |
|Dialogic  <br/> |DMG3000  <br/> | BRI Q.SIG  <br/> |
|NET  <br/> |VX1200  <br/> | T1 Q.SIG  <br/> |
|Sonus  <br/> |SBC 1000/2000 2.2.1 or later  <br/> | TDM Signaling (ISDN): AT&amp;T 4ESS/5ESS, Nortel DMS- 100, Euro ISDN (ETSI 300-102), QSIG, NTT InsNet (Japan), ANSI National ISDN-2 (NI-2)  <br/>  TDM Signaling (CAS): T1 CAS (E&amp;M, Loop start); E1 CAS (R2)  <br/> |
|Quintum  <br/> |Tenor DX Series  <br/> | T1 Q.SIG  <br/> |
   
## Supported PBXs when using an AudioCodes VoIP gateway
<a name="supPBXAudio"> </a>

The following table shows the PBXs that are supported using AudioCodes VoIP gateways, including MediaPack-114 FXO, MediaPack-118 FXO, and Mediant 2000.
  
**PBXs supported with an AudioCodes VoIP gateway**

|**PBX manufacturer**|**PBX model/type**|**AudioCodes model "x" - replace with 4 or 8 per need "y" - replace with 1, 2, 4, 8 or 16 per need**|
|:-----|:-----|:-----|
|Alcatel  <br/> |OmniPCX 4400  <br/> | MediaPack 11x/FXO/AC/SIP-0  <br/>  Mediant2000/ySpans/SIP  <br/> |
|Aastra  <br/> |M1000, M2000  <br/> | Mediant2000/ySpans/SIP  <br/> |
|Avaya  <br/> |Definity G3  <br/> | MediaPack 11x/FXO/AC/SIP-0  <br/>  Mediant1000/ySpans/SIP  <br/>  Mediant2000/ySpans/SIP  <br/> |
|Avaya  <br/> |Magix/Merlin  <br/> | MediaPack 11x/FXO/AC/SIP-0  <br/> |
|Avaya  <br/> |S8300  <br/> | MediaPack 11x/FXO/AC/SIP-0  <br/>  Mediant1000/ySpans/SIP  <br/>  Mediant2000/ySpans/SIP  <br/> |
|Avaya  <br/> |S8700  <br/> | MediaPack 11x/FXO/AC/SIP-0  <br/>  Mediant1000/ySpans/SIP  <br/>  Mediant2000/ySpans/SIP  <br/> |
|Avaya  <br/> |IP Office  <br/> | MediaPack 11x/FXO/AC/SIP-0  <br/>  Mediant2000/ySpans/SIP  <br/> |
|Cisco  <br/> |CallManager 4.x  <br/> | Mediant1000/IP-to-IP  <br/>  Mediant2000/IP-to-IP  <br/> |
|NEC  <br/> |Electra Elite  <br/> | MediaPack 11x/FXO/AC/SIP-0  <br/> |
|NEC  <br/> |NEAX2400  <br/> | MediaPack 11x/FXO/AC/SIP-0  <br/>  Mediant2000/ySpans/SIP/RS232  <br/> |
|NeXspan  <br/> |S  <br/> | MediaPack 11x/FXO/AC/SIP-0  <br/> |
|Nortel  <br/> |Communication Server-1000M, 1000S, 1000E  <br/> | Mediant1000/ySpans/SIP  <br/>  Mediant2000/ySpans/SIP  <br/> |
|Nortel  <br/> |Meridian 11c, 51c, 61c, 81c  <br/> | Mediant1000/ySpans/SIP  <br/>  Mediant2000/ySpans/SIP  <br/> |
|Panasonic  <br/> |KX-TES824, KX-TEA308  <br/> | MediaPack 11x/FXO/AC/SIP-0  <br/> |
|Panasonic  <br/> |KX-TDA30, KX-TDA100, KX-TDA200, KX-TDA600  <br/> | MediaPack 11x/FXO/AC/SIP-0  <br/> |
|Shortel  <br/> |IP Telephony System  <br/> | MediaPack 11x/FXO/AC/SIP-0  <br/> |
|Siemens  <br/> |HiCom 150E  <br/> | MediaPack 11x/FXO/AC/SIP-0  <br/> |
|Siemens  <br/> |HiPath 3550  <br/> | MediaPack 11x/FXO/AC/SIP-0  <br/> |
|Siemens  <br/> |HiPath 4000  <br/> | MediaPack 11x/FXO/AC/SIP-0  <br/>  Mediant1000/ySpans/SIP  <br/>  Mediant2000/ySpans/SIP  <br/> |
|Tadiran Telecom  <br/> |Coral Flexicom, Coral IPX  <br/> | MediaPack 11x/FXO/AC/SIP-0  <br/>  Mediant1000/ySpans/SIP  <br/>  Mediant2000/ySpans/SIP  <br/> |
   
## Supported PBXs when using a Dialogic VoIP gateway
<a name="supDialogic"> </a>

Each Dialogic VoIP gateway model supports different PBXs. The following tables show the PBX manufacturer and model and which Dialogic VoIP gateway can be used. Each VoIP gateway uses different signaling methods, densities, and protocols.
  
### PBXs supported when using a DMG1000 series Media Gateway
<a name="supDMG1000"> </a>

The following table shows the PBXs that are supported with the low-density Dialogic Media Gateway (DMG1000). However, when an analog DMG1000 is used, supplemental signaling (RS232 SMDI, MD110, MCI protocols, or Inband DTMF signaling) is required.
  
**PBXs supported when using a low-density Dialogic DMG1000 series VoIP gateway**

|**PBX manufacturer**|**PBX model/type**|**DMG model and additional signaling**|
|:-----|:-----|:-----|
|Aastra  <br/> |Aastra MD110 (formerly Ericsson MD110)  <br/> |DMG1008LSW  <br/> Analog connectivity using the MD110 RS232 protocol  <br/> |
|Alcatel  <br/> |Omni PCX 4400  <br/> |DMG1008LSW  <br/> |
|Avaya  <br/> |Definity G3 S8100, S8300, S8700, and S8710 (Communications Mgr SW V2.0 or later versions)  <br/> |DMG1008DNIW  <br/> |
|Intercom  <br/> | <br/> |DMG1008LSW  <br/> Analog connectivity using SMDI serial protocol  <br/> |
|Mitel  <br/> |SX-200D, SX-200 Light, SX-2000 Light, SX-2000 S, SX-2000 VS, SX-200 ICP  <br/> |DMG1008MTLDNIW  <br/> |
|NEC  <br/> |2000, 2400, 2400 IPX  <br/> |DMG1008DNIW  <br/> |
|Nortel  <br/> |Meridian 1 - Option 11, 21, 21A, 51, 61, 71, and 81  <br/> Meridian SL1 - Generic X11, Release 15 or later versions  <br/> Nortel Communication Server - 1000M, 1000S, 1000E with V3.0 or later versions  <br/> |DMG1008DNIW  <br/> |
|Nortel  <br/> |SL 100  <br/> |DMG1008LSW  <br/> Analog connectivity using SMDI serial protocol  <br/> |
|Siemens  <br/> |HiCom 300E CS  <br/> |DMG1008DNIW  <br/> |
|Siemens  <br/> |HiCom 300E (European)  <br/> |DMG1008LSW  <br/> Analog connectivity using Inband DTMF signaling  <br/> |
|Siemens/ROLM  <br/> |8000 (SW release 80003 or later versions)          9000 (All versions)  <br/> 9751 (All versions of SW release 9005)  <br/> 9751 (SW release 9006.4 or later versions)  <br/> |DMG1008RLMDNIW  <br/> |
|Siemens  <br/> |HiPath 4000  <br/> |DMG1008LSW  <br/> |
|Toshiba  <br/> |CTX (SW version AR1ME021.00)  <br/> |DMG1008LSW  <br/> |
|Others  <br/> |Various  <br/> |DMG1008LSW  <br/> Analog connectivity using either Inband DTMF or SMDI  <br/> |
   
### PBXs supported when using a DMG 2000 series Media Gateway
<a name="supDMG2000"> </a>

The following table shows the PBXs that are supported with the T1/E1 Dialogic Media Gateway (DMG2000). The DMG2000 gateway, which comes in single span (DMG2030DTIQ), dual span (DMG2060DTIQ), or quad span (DMG2120DTIQ) densities, supports the following protocols:
  
- T1 CAS
    
- T1 Q.SIG
    
- E1 Q.SIG
    
- T1 NI-2
    
- T1 5ESS
    
- T1 DMS100
    
If Channel Associated Signaling (CAS) signaling is used, supplemental signaling (RS232 SMDI, MD110, MCI protocols, or Inband DTMF signaling) is required. If Q.SIG signaling is used, the PBX must support the supplemental services that are associated with calling and called party information and the call transfer capabilities required by Unified Messaging.
  
**PBXs supported with the DMG2000 Media Gateway**

|**PBX manufacturer**|**PBX model/type**|**Required software version**|**Protocol and additional signaling**|
|:-----|:-----|:-----|:-----|
|Alcatel  <br/> |Omni PCX 4400  <br/> |Version 3.2.712.5  <br/> |T1 Q.SIG  <br/> E1 Q.SIG  <br/> |
|Avaya  <br/> |Definity G3  <br/> |Version 3 or later  <br/> |T1 CAS  <br/> |
|Avaya  <br/> |S8500  <br/> |Manager SW V2.0 or later versions  <br/> |T1 CAS  <br/> T1 Q.SIG  <br/> E1 Q.SIG  <br/> |
|Ericsson  <br/> |MD110  <br/> |Release MX1 TSW R2A (BC13)  <br/> |E1 Q.SIG  <br/> |
|Intercom  <br/> | <br/> | <br/> |CAS (w/ SMDI serial protocol)  <br/> |
|NEC  <br/> |2400 IMX  <br/> |Release 5200 Dec. 92 1b or later versions  <br/> |CAS (w/ MCI serial protocol)  <br/> |
|NEC  <br/> |2400 IPX  <br/> |R17 Release 03.46.001  <br/> |T1 Q.SIG  <br/> |
|Nortel  <br/> |Meridian 1 - Option 11  <br/> |Release 15 or later versions, and options 19 and 46 are required  <br/> |T1 Q.SIG  <br/> E1 Q.SIG  <br/> |
|Nortel  <br/> |Communication Server 1000  <br/> |Version 2121, Release 4  <br/> |T1 Q.SIG  <br/> E1 Q.SIG  <br/> |
|Siemens  <br/> |HiCom 300E CS  <br/> |Release 9006.4 or later (Note: North American software load only)  <br/> |T1 CAS  <br/> |
|Siemens  <br/> |HiPath 4000  <br/> |V2 SMR 9 SMPO  <br/> |T1 Q.SIG  <br/> E1 Q.SIG  <br/> |
|Mitel  <br/> |SX-2000 S, SX-2000 VS  <br/> |LW 34  <br/> |T1 Q.SIG  <br/> E1 Q.SIG  <br/> |
|Mitel  <br/> |3300  <br/> |Version 5.1.4.8  <br/> |T1 Q.SIG  <br/> E1 Q.SIG  <br/> |
   
### PBXs supported when using a DMG4008BRI series Media Gateway
<a name="supDMG3000"> </a>

The DMG4000 series Media Gateway comes with several TDM interface options. The DMG4008BRI supports 4-port/8-channel densities and supports the following protocols:
  
- ISDN BRI Q.SIG
    
- ETSI-DSS1 (Euro ISDN)
    
- NET 3 (Belgium)
    
- VN3 (France)
    
- 1TR6 (Germany)
    
- INS-64 (Japan)
    
- 5ESS Custom (North America - AT&amp;T)
    
- National ISDN (NI1 - North America)
    
The following table shows the PBXs that are supported using a Dialogic 4000 Media Gateway Series (DMG4008).
  
**PBXs supported using a DMG4008BRI Media Gateway**

|**PBX manufacturer**|**PBX model/type**|**Required software version**|**Protocol and additional signaling**|
|:-----|:-----|:-----|:-----|
|Siemens  <br/> |HiCom 300  <br/> |SA300-V3.05  <br/> |BRI-Q.SIG (ECMAV2)  <br/> |
|Siemens  <br/> |HiPath 4000  <br/> |S.0 B4400  <br/> |BRI-Q.SIG (ECMAV2)  <br/> |
   
## Supported IP PBXs
<a name="supIPPBX"> </a>

IP PBXs are also supported by Unified Messaging. The following table shows the IP PBXs that are supported using a direct SIP connection to Unified Messaging.
  
**IP PBXs supported when using a direct SIP connection**

|**PBX manufacturer**|**PBX model/type**|**Required software version**|
|:-----|:-----|:-----|
|Aastra  <br/> |MX-ONE  <br/> |4.0  <br/> |
|Avaya  <br/> |Aura  <br/> |5.2.1 with Service Pack 5 (SP5)  <br/> |
|Avaya  <br/> |Communication Server 2100  <br/> |CS2100 SE13  <br/> |
|Cisco  <br/> |Call Manager, Unified Communications Manager  <br/> |5.1, 6.x, 7.0 and8.0  <br/> |
   
## IP PBXs supported when using SIP media gateways
<a name="supIPPBXMediaGateway"> </a>

IP PBXs using SIP media gateways are also supported by Unified Messaging. The following table shows the IP PBXs that are supported using IP to IP capabilities of SIP media gateways to connect to Unified Messaging.
  
**IP PBXs supported when using a SIP media gateway**

|**PBX manufacturer**|**PBX model/type**|**SIP gateway model**|
|:-----|:-----|:-----|
|Cisco  <br/> |Call Manager 4.x  <br/> |AudioCodes Mediant 1000/2000 (IP-to-IP enabled)  <br/> |
   
## Exchange Unified Messaging, Office Communications Server 2007 R2, and Microsoft Lync Server
<a name="supLync"> </a>

For on-premises and hybrid deployments, Exchange Unified Messaging can be deployed together with Microsoft Office Communications Server 2007 R2, Microsoft Lync Server 2010 or Lync Server 2013 to provide voice messaging, Instant Messaging (IM), enhanced user presence, audio-video conferencing, and an integrated email and messaging experience for users in your organization. For more information, see:
  
- [Integrate Exchange 2013 UM with Lync Server](http://technet.microsoft.com/library/96fcb0dd-79ee-4e55-9e59-3ee7fbe3c4a1.aspx)
    
- [Microsoft Lync Server 2013](https://go.microsoft.com/fwlink/p/?LinkID=202010)
    
To find out more about the Microsoft Unified Communications Open Interoperability Program for enterprise telephony infrastructure, including finding qualified SIP PSTN gateways and IP PBXs and the process for telephony infrastructure vendors to join and participate in the program, see [Microsoft Unified Communications Open Interoperability Program](https://go.microsoft.com/fwlink/p/?linkId=132071).
  
