+++

description = ""
title = "f922e65f-baea-45c6-bdfa-0b6ab679bda8"
weight = 10
displayTitle = "bootmgfw.efi"
+++


{{< block "grid-1" >}}
{{< column "mt-2 pt-1">}}


# bootmgfw.efi ![:inline](/images/twitter_verified.png) 


### Description

This was provided by Microsoft and revoked May-23
- **UUID**: f922e65f-baea-45c6-bdfa-0b6ab679bda8
- **Created**: 2023-05-22
- **Author**: Michael Haag
- **Acknowledgement**:  | [](https://twitter.com/)

{{< button "https://github.com/magicsword-io/bootloaders/raw/main/bootloaders/2eb1ef37d6d0425c505df369802d5d54.bin" "Download" >}}
{{< tip "warning" >}}
This download link contains the Revoked Bootloader!

{{< /tip >}}

### Commands

```
bcdedit /copy &#34;{current}&#34; /d &#34;TheBoots&#34; | {% if ($_ -match &#39;{\S+}&#39;) { bcdedit /set $matches[0] path \windows\temp\bootmgfw.efi } }
```


| Use Case | Privileges | Operating System | 
|:---- | ---- | ---- |
| Persistence |  | 64-bit |



### Detections


{{< block "grid-3" >}}
{{< column >}}
#### YARA 🏹
{{< details "Expand" >}}

{{< button "https://github.com/magicsword-io/bootloaders/tree/main/detections/yara/yara-rules_bootloaders_strict.yar" "Exact Match" >}}{{< tip >}}with header and size limitation{{< /tip >}} 

{{< button "https://github.com/magicsword-io/bootloaders/tree/main/detections/yara/yara-rules_bootloaders.yar" "Threat Hunting" >}}{{< tip >}}without header and size limitation{{< /tip >}} 

{{< button "https://github.com/magicsword-io/bootloaders/tree/main/detections/yara/yara-rules_bootloaders_strict_renamed.yar" "Renamed" >}}{{< tip >}}for renamed bootloader files{{< /tip >}} 


{{< /details >}}
{{< /column >}}



{{< column >}}

#### Sigma 🛡️
{{< details "Expand" >}}
{{< button "https://github.com/magicsword-io/bootloaders/tree/main/detections/sigma/bootloader_load_win_vuln_bootloaders_names.yml" "Names" >}}{{< tip >}}detects loading using name only{{< /tip >}} 


{{< button "https://github.com/magicsword-io/bootloaders/tree/main/detections/sigma/bootloader_load_win_vuln_bootloaders.yml" "Hashes" >}}{{< tip >}}detects loading using hashes only{{< /tip >}} 

{{< /details >}}

{{< /column >}}


{{< column "mb-2" >}}

#### Sysmon 🔎
{{< details "Expand" >}}
{{< button "https://github.com/magicsword-io/bootloaders/tree/main/detections/sysmon/sysmon_config_vulnerable_hashes_block.xml" "Block" >}}{{< tip >}}on hashes{{< /tip >}} 

{{< button "https://github.com/magicsword-io/bootloaders/tree/main/detections/sysmon/sysmon_config_vulnerable_hashes.xml" "Alert" >}}{{< tip >}}on hashes{{< /tip >}} 

{{< /details >}}

{{< /column >}}
{{< /block >}}


### Resources
<br>
<li><a href="https://uefi.org/revocationlistfile">https://uefi.org/revocationlistfile</a></li>
<li><a href="https://support.microsoft.com/en-gb/topic/microsoft-guidance-for-applying-secure-boot-dbx-update-kb4575994-e3b9e4cb-a330-b3ba-a602-15083965d9ca">https://support.microsoft.com/en-gb/topic/microsoft-guidance-for-applying-secure-boot-dbx-update-kb4575994-e3b9e4cb-a330-b3ba-a602-15083965d9ca</a></li>
<br>

### CVE

<li><a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=Black Lotus Microsoft Windows 8">Black Lotus Microsoft Windows 8</a></li>

### Known Vulnerable Samples

| Property           | Value |
|:-------------------|:------|
| Filename           | bootmgfw.efi |
| MD5                | [2eb1ef37d6d0425c505df369802d5d54](https://www.virustotal.com/gui/file/2eb1ef37d6d0425c505df369802d5d54) |
| SHA1               | [8568540072aa5aead8d761d4baa459e4f9a222b2](https://www.virustotal.com/gui/file/8568540072aa5aead8d761d4baa459e4f9a222b2) |
| SHA256             | [9e14396bca7712b13a5f0b209c8633d754afc3bf577b42ef78304581ddd4e02f](https://www.virustotal.com/gui/file/9e14396bca7712b13a5f0b209c8633d754afc3bf577b42ef78304581ddd4e02f) |
| Authentihash MD5   | [170d26c08c0bd42cabe41e7223cf1a3b](https://www.virustotal.com/gui/search/authentihash%253A170d26c08c0bd42cabe41e7223cf1a3b) |
| Authentihash SHA1  | [026ce5f4baea28c655be66c8ac4873ddcd2fb089](https://www.virustotal.com/gui/search/authentihash%253A026ce5f4baea28c655be66c8ac4873ddcd2fb089) |
| Authentihash SHA256| [8d5332b350577ab7b1987f93fda104b2090f6a62e262214264f554b6163e8050](https://www.virustotal.com/gui/search/authentihash%253A8d5332b350577ab7b1987f93fda104b2090f6a62e262214264f554b6163e8050) |
| RichPEHeaderHash MD5   | [fa6462badb7aa537a9d3ecf604e9fbd7](https://www.virustotal.com/gui/search/rich_pe_header_hash%253Afa6462badb7aa537a9d3ecf604e9fbd7) |
| RichPEHeaderHash SHA1  | [caefdafc6f3620830b306d429c83bb077f6bdaa4](https://www.virustotal.com/gui/search/rich_pe_header_hash%253Acaefdafc6f3620830b306d429c83bb077f6bdaa4) |
| RichPEHeaderHash SHA256| [4689fe3d6e35db99759219db2adef6cefa62105e8b636c0c5bd2a6bec395e471](https://www.virustotal.com/gui/search/rich_pe_header_hash%253A4689fe3d6e35db99759219db2adef6cefa62105e8b636c0c5bd2a6bec395e471) |
| Company           | Microsoft Corporation |
| Description       | Boot Manager |
| Product           | Microsoft® Windows® Operating System |
| OriginalFilename  | bootmgr.exe |

#### Certificates

{{< details "Expand" >}}
###### Certificate 610bbbd8000000000005
| Field                             | Value                      |
|-----------------------------------|----------------------------|
| ToBeSigned (TBS) MD5              | 158438012e4dcd69b27b762c9358cfa2  |
| ToBeSigned (TBS) SHA1             | 684ac167849404a4101f166b759f291a43d5f749 |
| ToBeSigned (TBS) SHA256           | 95b37dd7079bf6836ab18482231be07fb3c05055af99691f8c64c6ad26eb8f9c |
| Subject                           | C=US, ST=Washington, L=Redmond, O=Microsoft Corporation, CN=Microsoft Windows |
| ValidFrom                         | 2012-04-09 20:55:50 |
| ValidTo                           | 2013-07-09 20:55:50 |
| Signature                         | c7f34d30f6c0451fb6ababdce5203035c20b7c75b16784adb0aa9ed8f647c02df4ce8d8277b8e356e3286e4dc0d444172dea83b9af9c6133c491e53680024d6bac0d985d6dfe776988ccb337b35abb32a02b50413514a576dc932b2a4ae2aef96330041e040480e3b1cbf06cd6910cf79ead3ecd332a9bb7156c2d9976e5dfac8b5b59d82ea33a4826470663dfad599e137468da7bd3037243e0238b96c1f99ea1299faa898dd854f812f8834697b7c5991d2e1656db4e2f56d8bc2077e7bb7d886d4fb6907c555c6d54089724435ac3345b1b6dbb605300ba83412517394dcd3b6c82df5013c6f57fcb1e03919b63469dd7606f3fbae8242658f19ab174b03c |
| SignatureAlgorithmOID             | 1.2.840.113549.1.1.11 |
| IsCertificateAuthority            | False |
| SerialNumber                      | 610bbbd8000000000005 |
| Version                           | 3 |
###### Certificate 61077656000000000008
| Field                             | Value                      |
|-----------------------------------|----------------------------|
| ToBeSigned (TBS) MD5              | 30a3f0b64324ed7f465e7fc618cb69e7  |
| ToBeSigned (TBS) SHA1             | 002de3561519b662c5e3f5faba1b92c403fb7c41 |
| ToBeSigned (TBS) SHA256           | 4e80be107c860de896384b3eff50504dc2d76ac7151df3102a4450637a032146 |
| Subject                           | C=US, ST=Washington, L=Redmond, O=Microsoft Corporation, CN=Microsoft Windows Production PCA 2011 |
| ValidFrom                         | 2011-10-19 18:41:42 |
| ValidTo                           | 2026-10-19 18:51:42 |
| Signature                         | 14fc7c7151a579c26eb2ef393ebc3c520f6e2b3f101373fea868d048a6344d8a960526ee3146906179d6ff382e456bf4c0e528b8da1d8f8adb09d71ac74c0a36666a8cec1bd70490a81817a49bb9e240323676c4c15ac6bfe404c0ea16d3acc368ef62acdd546c503058a6eb7cfe94a74e8ef4ec7c867357c2522173345af3a38a56c804da0709edf88be3cef47e8eaef0f60b8a08fb3fc91d727f53b8ebbe63e0e33d3165b081e5f2accd16a49f3da8b19bc242d090845f541dff89eaba1d47906fb0734e419f409f5fe5a12ab21191738a2128f0cede73395f3eab5c60ecdf0310a8d309e9f4f69685b67f51886647198da2b0123d812a680577bb914c627bb6c107c7ba7a8734030e4b627a99e9cafcce4a37c92da4577c1cfe3ddcb80f5afad6c4b30285023aeab3d96ee4692137de81d1f675190567d393575e291b39c8ee2de1cde445735bd0d2ce7aab1619824658d05e9d81b367af6c35f2bce53f24e235a20a7506f6185699d4782cd1051bebd088019daa10f105dfba7e2c63b7069b2321c4f9786ce2581706362b911203cca4d9f22dbaf9949d40ed1845f1ce8a5c6b3eab03d370182a0a6ae05f47d1d5630a32f2afd7361f2a705ae5425908714b57ba7e8381f0213cf41cc1c5b990930e88459386e9b12099be98cbc595a45d62d6a0630820bd7510777d3df345b99f979fcb57806f33a904cf77a4621c597e |
| SignatureAlgorithmOID             | 1.2.840.113549.1.1.11 |
| IsCertificateAuthority            | True |
| SerialNumber                      | 61077656000000000008 |
| Version                           | 3 |

{{< /details >}}
#### Imports
{{< details "Expand" >}}
* 

{{< /details >}}
#### Imports
{{< details "Expand" >}}
* 

{{< /details >}}
#### ImportedFunctions
{{< details "Expand" >}}

{{< /details >}}
#### ExportedFunctions
{{< details "Expand" >}}

{{< /details >}}

#### Signature
{{< details "Expand" >}}
```
{
  "Certificates": [
    {
      "IsCertificateAuthority": false,
      "SerialNumber": "610bbbd8000000000005",
      "Signature": "c7f34d30f6c0451fb6ababdce5203035c20b7c75b16784adb0aa9ed8f647c02df4ce8d8277b8e356e3286e4dc0d444172dea83b9af9c6133c491e53680024d6bac0d985d6dfe776988ccb337b35abb32a02b50413514a576dc932b2a4ae2aef96330041e040480e3b1cbf06cd6910cf79ead3ecd332a9bb7156c2d9976e5dfac8b5b59d82ea33a4826470663dfad599e137468da7bd3037243e0238b96c1f99ea1299faa898dd854f812f8834697b7c5991d2e1656db4e2f56d8bc2077e7bb7d886d4fb6907c555c6d54089724435ac3345b1b6dbb605300ba83412517394dcd3b6c82df5013c6f57fcb1e03919b63469dd7606f3fbae8242658f19ab174b03c",
      "SignatureAlgorithmOID": "1.2.840.113549.1.1.11",
      "Subject": "C=US, ST=Washington, L=Redmond, O=Microsoft Corporation, CN=Microsoft Windows",
      "TBS": {
        "MD5": "158438012e4dcd69b27b762c9358cfa2",
        "SHA1": "684ac167849404a4101f166b759f291a43d5f749",
        "SHA256": "95b37dd7079bf6836ab18482231be07fb3c05055af99691f8c64c6ad26eb8f9c"
      },
      "ValidFrom": "2012-04-09 20:55:50",
      "ValidTo": "2013-07-09 20:55:50",
      "Version": 3
    },
    {
      "IsCertificateAuthority": true,
      "SerialNumber": "61077656000000000008",
      "Signature": "14fc7c7151a579c26eb2ef393ebc3c520f6e2b3f101373fea868d048a6344d8a960526ee3146906179d6ff382e456bf4c0e528b8da1d8f8adb09d71ac74c0a36666a8cec1bd70490a81817a49bb9e240323676c4c15ac6bfe404c0ea16d3acc368ef62acdd546c503058a6eb7cfe94a74e8ef4ec7c867357c2522173345af3a38a56c804da0709edf88be3cef47e8eaef0f60b8a08fb3fc91d727f53b8ebbe63e0e33d3165b081e5f2accd16a49f3da8b19bc242d090845f541dff89eaba1d47906fb0734e419f409f5fe5a12ab21191738a2128f0cede73395f3eab5c60ecdf0310a8d309e9f4f69685b67f51886647198da2b0123d812a680577bb914c627bb6c107c7ba7a8734030e4b627a99e9cafcce4a37c92da4577c1cfe3ddcb80f5afad6c4b30285023aeab3d96ee4692137de81d1f675190567d393575e291b39c8ee2de1cde445735bd0d2ce7aab1619824658d05e9d81b367af6c35f2bce53f24e235a20a7506f6185699d4782cd1051bebd088019daa10f105dfba7e2c63b7069b2321c4f9786ce2581706362b911203cca4d9f22dbaf9949d40ed1845f1ce8a5c6b3eab03d370182a0a6ae05f47d1d5630a32f2afd7361f2a705ae5425908714b57ba7e8381f0213cf41cc1c5b990930e88459386e9b12099be98cbc595a45d62d6a0630820bd7510777d3df345b99f979fcb57806f33a904cf77a4621c597e",
      "SignatureAlgorithmOID": "1.2.840.113549.1.1.11",
      "Subject": "C=US, ST=Washington, L=Redmond, O=Microsoft Corporation, CN=Microsoft Windows Production PCA 2011",
      "TBS": {
        "MD5": "30a3f0b64324ed7f465e7fc618cb69e7",
        "SHA1": "002de3561519b662c5e3f5faba1b92c403fb7c41",
        "SHA256": "4e80be107c860de896384b3eff50504dc2d76ac7151df3102a4450637a032146"
      },
      "ValidFrom": "2011-10-19 18:41:42",
      "ValidTo": "2026-10-19 18:51:42",
      "Version": 3
    }
  ],
  "CertificatesInfo": "",
  "Signer": [
    {
      "Issuer": "C=US, ST=Washington, L=Redmond, O=Microsoft Corporation, CN=Microsoft Windows Production PCA 2011",
      "SerialNumber": "610bbbd8000000000005",
      "Version": 1
    }
  ],
  "SignerInfo": ""
}
```

{{< /details >}}
-----



[*source*](https://github.com/magicsword-io/bootloaders/tree/main/yaml/f922e65f-baea-45c6-bdfa-0b6ab679bda8.yaml)

*last_updated:* 2023-08-03








{{< /column >}}
{{< /block >}}
