+++

description = ""
title = "50cfaec9-55f8-49df-aa3e-b9ec3f4f4ff3"
weight = 10
displayTitle = "mhyprot.sys"
+++


{{< block "grid-1" >}}
{{< column "mt-2 pt-1">}}


# mhyprot.sys ![:inline](/images/twitter_verified.png) 

### Description

mhyprot.sys is a vulnerable driver and more information will be added as found.
- **UUID**: 50cfaec9-55f8-49df-aa3e-b9ec3f4f4ff3
- **Created**: 2023-01-09
- **Author**: Michael Haag
- **Acknowledgement**:  | [](https://twitter.com/)

{{< button "https://github.com/khulnasoft-lab/mitigate-drivers/raw/main/drivers/4b817d0e7714b9d43db43ae4a22a161e.bin" "Download" >}}{{< button "https://www.khulnasoft.com/premium" "Block" "red" >}}
{{< tip "warning" >}}
This download link contains the vulnerable driver!

{{< /tip >}}

### Commands

```
sc.exe create mhyprot.sys binPath=C:\windows\temp\mhyprot.sys type=kernel &amp;&amp; sc.exe start mhyprot.sys
```


| Use Case | Privileges | Operating System | 
|:---- | ---- | ---- |
| Elevate privileges | kernel | Windows 10 |



### Detections


{{< block "grid-3" >}}
{{< column >}}
#### YARA 🏹
{{< details "Expand" >}}

{{< button "https://github.com/khulnasoft-lab/mitigate-drivers/tree/main/detections/yara/yara-rules_vuln_drivers_strict.yar" "Exact Match" >}}{{< tip >}}with header and size limitation{{< /tip >}} 

{{< button "https://github.com/khulnasoft-lab/mitigate-drivers/tree/main/detections/yara/yara-rules_vuln_drivers.yar" "Threat Hunting" >}}{{< tip >}}without header and size limitation{{< /tip >}} 

{{< button "https://github.com/khulnasoft-lab/mitigate-drivers/tree/main/detections/yara/yara-rules_vuln_drivers_strict_renamed.yar" "Renamed" >}}{{< tip >}}for renamed driver files{{< /tip >}} 


{{< /details >}}
{{< /column >}}



{{< column >}}

#### Sigma 🛡️
{{< details "Expand" >}}
{{< button "https://github.com/khulnasoft-lab/mitigate-drivers/tree/main/detections/sigma/driver_load_win_vuln_drivers_names.yml" "Names" >}}{{< tip >}}detects loading using name only{{< /tip >}} 


{{< button "https://github.com/khulnasoft-lab/mitigate-drivers/tree/main/detections/sigma/driver_load_win_vuln_drivers.yml" "Hashes" >}}{{< tip >}}detects loading using hashes only{{< /tip >}} 

{{< /details >}}

{{< /column >}}


{{< column "mb-2" >}}

#### Sysmon 🔎
{{< details "Expand" >}}
{{< button "https://github.com/khulnasoft-lab/mitigate-drivers/tree/main/detections/sysmon/sysmon_config_vulnerable_hashes_block.xml" "Block" >}}{{< tip >}}on hashes{{< /tip >}} 

{{< button "https://github.com/khulnasoft-lab/mitigate-drivers/tree/main/detections/sysmon/sysmon_config_vulnerable_hashes.xml" "Alert" >}}{{< tip >}}on hashes{{< /tip >}} 

{{< /details >}}

{{< /column >}}
{{< /block >}}


### Resources
<br>
<li><a href=" https://github.com/jbaines-r7/dellicious"> https://github.com/jbaines-r7/dellicious</a></li>
<li><a href=" https://www.rapid7.com/blog/post/2021/12/13/driver-based-attacks-past-and-present/"> https://www.rapid7.com/blog/post/2021/12/13/driver-based-attacks-past-and-present/</a></li>
<li><a href="https://github.com/elastic/protections-artifacts/blob/932baf346cc8a743f1963ad3d4565b42ed17bebe/yara/rules/Windows_VulnDriver_Mhyprot.yar">https://github.com/elastic/protections-artifacts/blob/932baf346cc8a743f1963ad3d4565b42ed17bebe/yara/rules/Windows_VulnDriver_Mhyprot.yar</a></li>
<li><a href="https://github.com/jbaines-r7/dellicious and https://www.rapid7.com/blog/post/2021/12/13/driver-based-attacks-past-and-present/">https://github.com/jbaines-r7/dellicious and https://www.rapid7.com/blog/post/2021/12/13/driver-based-attacks-past-and-present/</a></li>
<br>


### Known Vulnerable Samples

| Property           | Value |
|:-------------------|:------|
| Filename           | mhyprot.sys |
| Creation Timestamp           | 2020-08-16 21:38:03 |
| MD5                | [4b817d0e7714b9d43db43ae4a22a161e](https://www.virustotal.com/gui/file/4b817d0e7714b9d43db43ae4a22a161e) |
| SHA1               | [0466e90bf0e83b776ca8716e01d35a8a2e5f96d3](https://www.virustotal.com/gui/file/0466e90bf0e83b776ca8716e01d35a8a2e5f96d3) |
| SHA256             | [509628b6d16d2428031311d7bd2add8d5f5160e9ecc0cd909f1e82bbbb3234d6](https://www.virustotal.com/gui/file/509628b6d16d2428031311d7bd2add8d5f5160e9ecc0cd909f1e82bbbb3234d6) |
| Authentihash MD5   | [ff295de93e6b6dcc3938d50901a7240d](https://www.virustotal.com/gui/search/authentihash%253Aff295de93e6b6dcc3938d50901a7240d) |
| Authentihash SHA1  | [484c72dd4fd91083b249f3ccc733a3c8335e583f](https://www.virustotal.com/gui/search/authentihash%253A484c72dd4fd91083b249f3ccc733a3c8335e583f) |
| Authentihash SHA256| [0c7809ac1fa074408518ddc0ac118912c9cd43ed9c89213bc4d59043016b040c](https://www.virustotal.com/gui/search/authentihash%253A0c7809ac1fa074408518ddc0ac118912c9cd43ed9c89213bc4d59043016b040c) |
| RichPEHeaderHash MD5   | [ffdf660eb1ebf020a1d0a55a90712dfb](https://www.virustotal.com/gui/search/rich_pe_header_hash%253Affdf660eb1ebf020a1d0a55a90712dfb) |
| RichPEHeaderHash SHA1  | [3e905e3d061d0d59de61fcf39c994fcb0ec1bab3](https://www.virustotal.com/gui/search/rich_pe_header_hash%253A3e905e3d061d0d59de61fcf39c994fcb0ec1bab3) |
| RichPEHeaderHash SHA256| [2b3f99a94b7a7132854be769e27b331419c53989ef42f686d6f5ba09ddefefd6](https://www.virustotal.com/gui/search/rich_pe_header_hash%253A2b3f99a94b7a7132854be769e27b331419c53989ef42f686d6f5ba09ddefefd6) |

{{< button "https://github.com/khulnasoft-lab/mitigate-drivers/raw/main/drivers/4b817d0e7714b9d43db43ae4a22a161e.bin" "Download" >}} 

#### Certificates

{{< details "Expand" >}}
###### Certificate 05a7559541e0fdc678d79e3272468907
| Field                             | Value                      |
|-----------------------------------|----------------------------|
| ToBeSigned (TBS) MD5              | 3e83a7572d1c522dd9072ba6399029d7  |
| ToBeSigned (TBS) SHA1             | e2c2d59b70f028a66a8711bfa97f842475f84639 |
| ToBeSigned (TBS) SHA256           | 5a504a929cb21f72008d5d57bcd992a7cac13f6aa90cbb886b5ecd809e3b59dd |
| Subject                           | C=CN, L=Shanghai, O=miHoYo Co.,Ltd., OU=OPS, CN=miHoYo Co.,Ltd. |
| ValidFrom                         | 2019-04-08 00:00:00 |
| ValidTo                           | 2022-04-08 12:00:00 |
| Signature                         | 46a5e6f6c38a63b314f7e2677bb86d4bcd7839eef8e006048ddd58c6783ff0657456e61c800efb31966c611f7ca7d1de1785e006e3f4c0b24cb652842e42cbae016320a774724537fc30e8f09895fdb626daa26b5740c7538aa1df1f97dcab12c3a743c2048f6c9a754f66189ac0f21544399798fb780cd347c9cac0443c8d778736938e17cdd5eca8a2338d8171efd61e13c868dff862da9df4ca8c653a227e0971030aa7e6b44dc2199d1ebd9cae00c6f0a3e91bb883cc509fb297902ba5c13e5826071d92178ace51f1a0653b0445cf7ba17226401c92d7db4f67a37d1243f9094ad5f32873891ea5004a8cbfec77129d4955e344492aaee456f852001ded |
| SignatureAlgorithmOID             | 1.2.840.113549.1.1.5 |
| IsCertificateAuthority            | False |
| SerialNumber                      | 05a7559541e0fdc678d79e3272468907 |
| Version                           | 3 |
###### Certificate 611cb28a000000000026
| Field                             | Value                      |
|-----------------------------------|----------------------------|
| ToBeSigned (TBS) MD5              | 983a0c315a50542362f2bd6a5d71c8d0  |
| ToBeSigned (TBS) SHA1             | 8047f476001f5cb16a661d2a3fd0c3576168f5e2 |
| ToBeSigned (TBS) SHA256           | 5f6a519ed2e35cd0fa1cdfc90f4387162c36287bbf9e4d6648251d99542a9e83 |
| Subject                           | C=US, O=DigiCert Inc, OU=www.digicert.com, CN=DigiCert Assured ID Root CA |
| ValidFrom                         | 2011-04-15 19:41:37 |
| ValidTo                           | 2021-04-15 19:51:37 |
| Signature                         | 5cf5b22d02ceed01b53512d813f7aa4014c7a15ca08a55ed7e55ea6ac457176fd04722423658efc5ac61c5f62c52ce6ae6c80d85dab334420ea40225182672b92a4ea57e4b16f2a0e40c449ce24d9af474f0f927a6699031c244654348c74869d0fc8409f286140ac22996857f11eb8713176ed3ec6bff1d578ab17b1ea5a07ce9a27a68e5fac6b161d67263fa379163835599f81d614f0c6fa3f7bcb1152acc8d85e31417ef7e49443fb022c0f0acbe2fdbe10c86b0f4585c5a10a94bcdf3448a4652083e0a6210e9459504b78b8d4b074f500db7bbe7fb8ca27878c6c53b7663b2cfe521845a66fce04c79834ecfa8ee700586587cc29cd73ca3ad3c7e76625c87d0ed7cd5c55b1421f4be75a275d2e9e15ad020307841624d6b5e6e1b1710244ad8588775d015d762bbfd185665842561977faad49df4f35d6da031c2e19e02ac3e90c3327ee832903416d08b14cf95accee58c54a265b8bfed186a57073ed3e79a4a2f081a041c49871a8ae61b08a365d81c31c50d9cbab368ddf45076160675fec403e7d13edfdc862e10027e661296534e7af3365879b12042d8963f35be3f8ef2999743f5e40ce13c68728c8d49d75a52b573fb7a35943a61b08482c04885c19732d39b725fa0d2348f7ef0467cf28c7294c707b0d7b5b230b81965f09c8327b0a0abd0a2727e050fb3aeddb95b9b42bcc32663456b86f11d4643edc8 |
| SignatureAlgorithmOID             | 1.2.840.113549.1.1.5 |
| IsCertificateAuthority            | True |
| SerialNumber                      | 611cb28a000000000026 |
| Version                           | 3 |
###### Certificate 03019a023aff58b16bd6d5eae617f066
| Field                             | Value                      |
|-----------------------------------|----------------------------|
| ToBeSigned (TBS) MD5              | a752afee44f017e8d74e3f3eb7914ae3  |
| ToBeSigned (TBS) SHA1             | 8eca80a6b80e9c69dcef7745748524afb8019e2d |
| ToBeSigned (TBS) SHA256           | 82560fa7efec30b5ff82af643e6f3bf3d46868bbd5e7d76f93db185e9e3553a1 |
| Subject                           | C=US, O=DigiCert, CN=DigiCert Timestamp Responder |
| ValidFrom                         | 2014-10-22 00:00:00 |
| ValidTo                           | 2024-10-22 00:00:00 |
| Signature                         | 9d257e1b334db226815c9b86ce23200f8087e588ffffb1d46a2c31ed3a17197117cda91bbc5a1639009de36c84e45a40fbde06018c37fa9bb19d247efe20a457ad5bb79ab06026ea6957215d342f1f71b0839419056b359010a07b97c7f63fe7e21141a6bd62d9f0273d381d286f3a5209f0ec7062d3624bb0e073a692c0d38e31d82fe36d171306eee403b614abf38f43a7719d21dd14ca155d9241daf90f81d199740d26c40e7f1bb5f5a0f1c677062815e9d893e55516f0bb0aab1cdb5c482766c8a38b0a1ce595daaec42e59a061dddaf36da261e98a0b6dec1218bdf755544003922b6bc251c20a48afb0d46ee0f4140a3a1be38f3dcaaf6a8d7bdcd844 |
| SignatureAlgorithmOID             | 1.2.840.113549.1.1.5 |
| IsCertificateAuthority            | False |
| SerialNumber                      | 03019a023aff58b16bd6d5eae617f066 |
| Version                           | 3 |
###### Certificate 0fa8490615d700a0be2176fdc5ec6dbd
| Field                             | Value                      |
|-----------------------------------|----------------------------|
| ToBeSigned (TBS) MD5              | a9a31555bbc92b6033975c5428fb3679  |
| ToBeSigned (TBS) SHA1             | 47f4b9898631773231b32844ec0d49990ac4eb1e |
| ToBeSigned (TBS) SHA256           | c826846e4b1d73edb7561ab1b41c949354e237a91e82fe1be5b7e2e1701f52d1 |
| Subject                           | C=US, O=DigiCert Inc, OU=www.digicert.com, CN=DigiCert Assured ID Code Signing CA,1 |
| ValidFrom                         | 2011-02-11 12:00:00 |
| ValidTo                           | 2026-02-10 12:00:00 |
| Signature                         | 7b721d64ff88c83ac1b7e9e7a9c487bbdb9492d7905933fa2b87dea85b80253f138f9b831b7c43c4e68cdf393ec315ecb0da3b21257b24c1725db84791811346fa9c3f6a5138deb425cbf0abdfc528015479104624d1380f26a161904dbabd28e63ff1c4aa9bf6da35534fc9f23dd36cdc23edaaa04d6709f33a803d3cfb364c90e776a4ddf23abf56352fa24c65e8e0d4dad1c7c8916a2d234f373b199418d4d59c103cd5b11c19ff8fc86b9b9ef8ae9c999678d1cd9c51155b4226725a8d0a4a239240e886de22c2933ad49b68a6df297f06b93c0ebd9fc4869c82474271328609997209794b9d7169f541ff7f397764f1848dbe8b1eb27d68a3a590b10cff |
| SignatureAlgorithmOID             | 1.2.840.113549.1.1.5 |
| IsCertificateAuthority            | True |
| SerialNumber                      | 0fa8490615d700a0be2176fdc5ec6dbd |
| Version                           | 3 |
###### Certificate 06fdf9039603adea000aeb3f27bbba1b
| Field                             | Value                      |
|-----------------------------------|----------------------------|
| ToBeSigned (TBS) MD5              | 4e5ad189638cf52ba9cd881d4d44668c  |
| ToBeSigned (TBS) SHA1             | cdc115e98d798b33904c820d63cc1e1afc19251d |
| ToBeSigned (TBS) SHA256           | 37560fb9d548ab62cc3ed4669a4ab74828b5a108e67e829937ffb2d10a5f78dd |
| Subject                           | C=US, O=DigiCert Inc, OU=www.digicert.com, CN=DigiCert Assured ID CA,1 |
| ValidFrom                         | 2006-11-10 00:00:00 |
| ValidTo                           | 2021-11-10 00:00:00 |
| Signature                         | 46503ec9b72824a7381db65b29af52cf52e93147ab565c7bd50d0b41b3efec751f7438f2b25c61a29c95c350e482b923d1ba3a8672ad3878ac755d1717347247859456d1ebbb368477cc24a5f3041955a9e7e3e7ab62cdfb8b2d90c2c0d2b594bd5e4fb105d20e3d1aa9145ba6863162a8a833e49b39a7c4f5ce1d7876942573e42aabcf9c764bed5fc24b16e44b704c00891efcc579bc4c1257fe5fe11ebc025da8fefb07384f0dc65d91b90f6745cdd683ede7920d8db1698c4ffb59e0230fd2aaae007cee9c420ecf91d727b716ee0fc3bd7c0aa0ee2c08558522b8eb181a4dfc2a21ad49318347957771dcb11b4b4b1c109c7714c19d4f2f5a9508291026 |
| SignatureAlgorithmOID             | 1.2.840.113549.1.1.5 |
| IsCertificateAuthority            | True |
| SerialNumber                      | 06fdf9039603adea000aeb3f27bbba1b |
| Version                           | 3 |

{{< /details >}}
#### Imports
{{< details "Expand" >}}
* ntoskrnl.exe
* WDFLDR.SYS

{{< /details >}}
#### Imported Functions
{{< details "Expand" >}}
* NtQuerySystemInformation
* RtlInitUnicodeString
* ExAllocatePool
* ExAllocatePoolWithTag
* ExFreePoolWithTag
* IofCompleteRequest
* IoCreateDevice
* IoCreateSymbolicLink
* IoDeleteDevice
* IoDeleteSymbolicLink
* _wcsicmp
* RtlInitString
* RtlAnsiStringToUnicodeString
* RtlFreeUnicodeString
* IoGetDeviceObjectPointer
* ZwClose
* MmIsAddressValid
* ZwOpenDirectoryObject
* ZwQueryDirectoryObject
* ObReferenceObjectByName
* ZwQuerySystemInformation
* __C_specific_handler
* MmHighestUserAddress
* IoDriverObjectType
* KeQueryTimeIncrement
* KeStackAttachProcess
* KeUnstackDetachProcess
* PsGetProcessWow64Process
* PsGetProcessPeb
* MmUnlockPages
* MmGetSystemRoutineAddress
* MmUnmapLockedPages
* IoFreeMdl
* ZwTerminateProcess
* PsGetProcessImageFileName
* ObOpenObjectByPointer
* PsReferenceProcessFilePointer
* IoQueryFileDosDeviceName
* ZwQueryVirtualMemory
* MmProbeAndLockPages
* PsLookupProcessByProcessId
* MmMapLockedPagesSpecifyCache
* IoAllocateMdl
* IoGetCurrentProcess
* MmCopyVirtualMemory
* KeClearEvent
* KeSetEvent
* KeWaitForSingleObject
* MmMapLockedPages
* ObReferenceObjectByHandle
* PsSetCreateProcessNotifyRoutineEx
* PsSetCreateThreadNotifyRoutine
* PsRemoveCreateThreadNotifyRoutine
* PsSetLoadImageNotifyRoutine
* PsRemoveLoadImageNotifyRoutine
* ExEventObjectType
* ObRegisterCallbacks
* ObUnRegisterCallbacks
* ObGetFilterVersion
* IoThreadToProcess
* strcmp
* PsProcessType
* PsThreadType
* RtlGetVersion
* ObfReferenceObject
* ObGetObjectType
* ExEnumHandleTable
* ExfUnblockPushLock
* _snprintf
* vsprintf_s
* ZwCreateFile
* ZwWriteFile
* PsLookupThreadByThreadId
* NtQueryInformationThread
* PsGetThreadProcess
* DbgPrint
* KeDelayExecutionThread
* KdDisableDebugger
* KdChangeOption
* PsCreateSystemThread
* PsTerminateSystemThread
* KdDebuggerEnabled
* PsGetVersion
* KeInitializeEvent
* RtlCopyUnicodeString
* ObfDereferenceObject
* ExReleaseFastMutex
* ExAcquireFastMutex
* MmBuildMdlForNonPagedPool
* WdfVersionBindClass
* WdfVersionBind
* WdfVersionUnbind
* WdfVersionUnbindClass

{{< /details >}}
#### Exported Functions
{{< details "Expand" >}}

{{< /details >}}

#### Sections
{{< details "Expand" >}}
* .text
* .rdata
* .data
* .pdata
* PAGE
* INIT
* .upx0
* .reloc
* .rsrc

{{< /details >}}
#### Signature
{{< details "Expand" >}}
```
{
  "Certificates": [
    {
      "IsCertificateAuthority": false,
      "SerialNumber": "05a7559541e0fdc678d79e3272468907",
      "Signature": "46a5e6f6c38a63b314f7e2677bb86d4bcd7839eef8e006048ddd58c6783ff0657456e61c800efb31966c611f7ca7d1de1785e006e3f4c0b24cb652842e42cbae016320a774724537fc30e8f09895fdb626daa26b5740c7538aa1df1f97dcab12c3a743c2048f6c9a754f66189ac0f21544399798fb780cd347c9cac0443c8d778736938e17cdd5eca8a2338d8171efd61e13c868dff862da9df4ca8c653a227e0971030aa7e6b44dc2199d1ebd9cae00c6f0a3e91bb883cc509fb297902ba5c13e5826071d92178ace51f1a0653b0445cf7ba17226401c92d7db4f67a37d1243f9094ad5f32873891ea5004a8cbfec77129d4955e344492aaee456f852001ded",
      "SignatureAlgorithmOID": "1.2.840.113549.1.1.5",
      "Subject": "C=CN, L=Shanghai, O=miHoYo Co.,Ltd., OU=OPS, CN=miHoYo Co.,Ltd.",
      "TBS": {
        "MD5": "3e83a7572d1c522dd9072ba6399029d7",
        "SHA1": "e2c2d59b70f028a66a8711bfa97f842475f84639",
        "SHA256": "5a504a929cb21f72008d5d57bcd992a7cac13f6aa90cbb886b5ecd809e3b59dd",
        "SHA384": "72916ab6c7eb3f5cb7444b3d7d2ac8cb52944605477c5a0f181d060e4edb4c37ebe5eb3c0566dda9de2d2707636ec355"
      },
      "ValidFrom": "2019-04-08 00:00:00",
      "ValidTo": "2022-04-08 12:00:00",
      "Version": 3
    },
    {
      "IsCertificateAuthority": true,
      "SerialNumber": "611cb28a000000000026",
      "Signature": "5cf5b22d02ceed01b53512d813f7aa4014c7a15ca08a55ed7e55ea6ac457176fd04722423658efc5ac61c5f62c52ce6ae6c80d85dab334420ea40225182672b92a4ea57e4b16f2a0e40c449ce24d9af474f0f927a6699031c244654348c74869d0fc8409f286140ac22996857f11eb8713176ed3ec6bff1d578ab17b1ea5a07ce9a27a68e5fac6b161d67263fa379163835599f81d614f0c6fa3f7bcb1152acc8d85e31417ef7e49443fb022c0f0acbe2fdbe10c86b0f4585c5a10a94bcdf3448a4652083e0a6210e9459504b78b8d4b074f500db7bbe7fb8ca27878c6c53b7663b2cfe521845a66fce04c79834ecfa8ee700586587cc29cd73ca3ad3c7e76625c87d0ed7cd5c55b1421f4be75a275d2e9e15ad020307841624d6b5e6e1b1710244ad8588775d015d762bbfd185665842561977faad49df4f35d6da031c2e19e02ac3e90c3327ee832903416d08b14cf95accee58c54a265b8bfed186a57073ed3e79a4a2f081a041c49871a8ae61b08a365d81c31c50d9cbab368ddf45076160675fec403e7d13edfdc862e10027e661296534e7af3365879b12042d8963f35be3f8ef2999743f5e40ce13c68728c8d49d75a52b573fb7a35943a61b08482c04885c19732d39b725fa0d2348f7ef0467cf28c7294c707b0d7b5b230b81965f09c8327b0a0abd0a2727e050fb3aeddb95b9b42bcc32663456b86f11d4643edc8",
      "SignatureAlgorithmOID": "1.2.840.113549.1.1.5",
      "Subject": "C=US, O=DigiCert Inc, OU=www.digicert.com, CN=DigiCert Assured ID Root CA",
      "TBS": {
        "MD5": "983a0c315a50542362f2bd6a5d71c8d0",
        "SHA1": "8047f476001f5cb16a661d2a3fd0c3576168f5e2",
        "SHA256": "5f6a519ed2e35cd0fa1cdfc90f4387162c36287bbf9e4d6648251d99542a9e83",
        "SHA384": "5f014b60511ddab3247ef0b3c03fe82c622237ba76015e2911d1adc50dc632d56ebd1ee532f3c2b6cbfe68d80a2c91dc"
      },
      "ValidFrom": "2011-04-15 19:41:37",
      "ValidTo": "2021-04-15 19:51:37",
      "Version": 3
    },
    {
      "IsCertificateAuthority": false,
      "SerialNumber": "03019a023aff58b16bd6d5eae617f066",
      "Signature": "9d257e1b334db226815c9b86ce23200f8087e588ffffb1d46a2c31ed3a17197117cda91bbc5a1639009de36c84e45a40fbde06018c37fa9bb19d247efe20a457ad5bb79ab06026ea6957215d342f1f71b0839419056b359010a07b97c7f63fe7e21141a6bd62d9f0273d381d286f3a5209f0ec7062d3624bb0e073a692c0d38e31d82fe36d171306eee403b614abf38f43a7719d21dd14ca155d9241daf90f81d199740d26c40e7f1bb5f5a0f1c677062815e9d893e55516f0bb0aab1cdb5c482766c8a38b0a1ce595daaec42e59a061dddaf36da261e98a0b6dec1218bdf755544003922b6bc251c20a48afb0d46ee0f4140a3a1be38f3dcaaf6a8d7bdcd844",
      "SignatureAlgorithmOID": "1.2.840.113549.1.1.5",
      "Subject": "C=US, O=DigiCert, CN=DigiCert Timestamp Responder",
      "TBS": {
        "MD5": "a752afee44f017e8d74e3f3eb7914ae3",
        "SHA1": "8eca80a6b80e9c69dcef7745748524afb8019e2d",
        "SHA256": "82560fa7efec30b5ff82af643e6f3bf3d46868bbd5e7d76f93db185e9e3553a1",
        "SHA384": "e8b11408c88f877ade4ca51114a175fb5dfd2d18d2a66be547c1c9e080fa8f592c7870e30dfab1c04d234993dd0907f3"
      },
      "ValidFrom": "2014-10-22 00:00:00",
      "ValidTo": "2024-10-22 00:00:00",
      "Version": 3
    },
    {
      "IsCertificateAuthority": true,
      "SerialNumber": "0fa8490615d700a0be2176fdc5ec6dbd",
      "Signature": "7b721d64ff88c83ac1b7e9e7a9c487bbdb9492d7905933fa2b87dea85b80253f138f9b831b7c43c4e68cdf393ec315ecb0da3b21257b24c1725db84791811346fa9c3f6a5138deb425cbf0abdfc528015479104624d1380f26a161904dbabd28e63ff1c4aa9bf6da35534fc9f23dd36cdc23edaaa04d6709f33a803d3cfb364c90e776a4ddf23abf56352fa24c65e8e0d4dad1c7c8916a2d234f373b199418d4d59c103cd5b11c19ff8fc86b9b9ef8ae9c999678d1cd9c51155b4226725a8d0a4a239240e886de22c2933ad49b68a6df297f06b93c0ebd9fc4869c82474271328609997209794b9d7169f541ff7f397764f1848dbe8b1eb27d68a3a590b10cff",
      "SignatureAlgorithmOID": "1.2.840.113549.1.1.5",
      "Subject": "C=US, O=DigiCert Inc, OU=www.digicert.com, CN=DigiCert Assured ID Code Signing CA,1",
      "TBS": {
        "MD5": "a9a31555bbc92b6033975c5428fb3679",
        "SHA1": "47f4b9898631773231b32844ec0d49990ac4eb1e",
        "SHA256": "c826846e4b1d73edb7561ab1b41c949354e237a91e82fe1be5b7e2e1701f52d1",
        "SHA384": "86f49574f368a561914a52d7ae043ec6784ef8c718960700f834e123594605d25d39f1ad45f1eb5052c9567f3edd0e16"
      },
      "ValidFrom": "2011-02-11 12:00:00",
      "ValidTo": "2026-02-10 12:00:00",
      "Version": 3
    },
    {
      "IsCertificateAuthority": true,
      "SerialNumber": "06fdf9039603adea000aeb3f27bbba1b",
      "Signature": "46503ec9b72824a7381db65b29af52cf52e93147ab565c7bd50d0b41b3efec751f7438f2b25c61a29c95c350e482b923d1ba3a8672ad3878ac755d1717347247859456d1ebbb368477cc24a5f3041955a9e7e3e7ab62cdfb8b2d90c2c0d2b594bd5e4fb105d20e3d1aa9145ba6863162a8a833e49b39a7c4f5ce1d7876942573e42aabcf9c764bed5fc24b16e44b704c00891efcc579bc4c1257fe5fe11ebc025da8fefb07384f0dc65d91b90f6745cdd683ede7920d8db1698c4ffb59e0230fd2aaae007cee9c420ecf91d727b716ee0fc3bd7c0aa0ee2c08558522b8eb181a4dfc2a21ad49318347957771dcb11b4b4b1c109c7714c19d4f2f5a9508291026",
      "SignatureAlgorithmOID": "1.2.840.113549.1.1.5",
      "Subject": "C=US, O=DigiCert Inc, OU=www.digicert.com, CN=DigiCert Assured ID CA,1",
      "TBS": {
        "MD5": "4e5ad189638cf52ba9cd881d4d44668c",
        "SHA1": "cdc115e98d798b33904c820d63cc1e1afc19251d",
        "SHA256": "37560fb9d548ab62cc3ed4669a4ab74828b5a108e67e829937ffb2d10a5f78dd",
        "SHA384": "173bfb77183785621ef15f43ea807338cea6a02e8183317d9ef050c7237adda3fa2a5bdcd5a4c96da9f2c55900675b9f"
      },
      "ValidFrom": "2006-11-10 00:00:00",
      "ValidTo": "2021-11-10 00:00:00",
      "Version": 3
    }
  ],
  "CertificatesInfo": "",
  "Signer": [
    {
      "Issuer": "C=US, O=DigiCert Inc, OU=www.digicert.com, CN=DigiCert Assured ID Code Signing CA,1",
      "SerialNumber": "05a7559541e0fdc678d79e3272468907",
      "Version": 1
    }
  ],
  "SignerInfo": ""
}
```

{{< /details >}}
-----



[*source*](https://github.com/khulnasoft-lab/mitigate-drivers/tree/main/yaml/50cfaec9-55f8-49df-aa3e-b9ec3f4f4ff3.yaml)

*last_updated:* 2024-12-10

{{< /column >}}
{{< /block >}}
