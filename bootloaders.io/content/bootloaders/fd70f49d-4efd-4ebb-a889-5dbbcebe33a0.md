+++

description = ""
title = "fd70f49d-4efd-4ebb-a889-5dbbcebe33a0"
weight = 10
displayTitle = "centos-7.9-shim-20200726-shimia32.efi"
+++


{{< block "grid-1" >}}
{{< column "mt-2 pt-1">}}


# centos-7.9-shim-20200726-shimia32.efi ![:inline](/images/twitter_verified.png) 


### Description

This was provided by Red Hat, Inc. and revoked Apr-21
- **UUID**: fd70f49d-4efd-4ebb-a889-5dbbcebe33a0
- **Created**: 2023-05-22
- **Author**: Michael Haag
- **Acknowledgement**:  | [](https://twitter.com/)

{{< button "https://github.com/magicsword-io/bootloaders/raw/main/bootloaders/.bin" "Download" >}}
{{< tip "warning" >}}
This download link contains the Revoked Bootloader!

{{< /tip >}}

### Commands

```
bcdedit /copy &#34;{current}&#34; /d &#34;TheBoots&#34; | {% if ($_ -match &#39;{\S+}&#39;) { bcdedit /set $matches[0] path \windows\temp\centos-7.9-shim-20200726-shimia32.efi } }
```


| Use Case | Privileges | Operating System | 
|:---- | ---- | ---- |
| Persistence |  | 32-bit |



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

<li><a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2020-14372">CVE-2020-14372</a></li>
<li><a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2020-25632">CVE-2020-25632</a></li>
<li><a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2020-25647">CVE-2020-25647</a></li>
<li><a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2020-27749">CVE-2020-27749</a></li>
<li><a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2020-27779">CVE-2020-27779</a></li>
<li><a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2021-3418">CVE-2021-3418</a></li>
<li><a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2021-20225">CVE-2021-20225</a></li>
<li><a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2021-20233">CVE-2021-20233</a></li>

### Known Vulnerable Samples

| Property           | Value |
|:-------------------|:------|
| Filename           | centos-7.9-shim-20200726-shimia32.efi |
| MD5                | [](https://www.virustotal.com/gui/file/) |
| SHA1               | [](https://www.virustotal.com/gui/file/) |
| SHA256             | [8C3A26B5831FF45BC3BCA44C2815951E2DA489A91BBCD295F12DFDBCED9958B9](https://www.virustotal.com/gui/file/8C3A26B5831FF45BC3BCA44C2815951E2DA489A91BBCD295F12DFDBCED9958B9) |
| Authentihash MD5   | [](https://www.virustotal.com/gui/search/authentihash%253A) |
| Authentihash SHA1  | [](https://www.virustotal.com/gui/search/authentihash%253A) |
| Authentihash SHA256| [398995770D21E9F66B90D69D1EDE16C9E58C0634B2F7D26B1F22501DD93FDAE5](https://www.virustotal.com/gui/search/authentihash%253A398995770D21E9F66B90D69D1EDE16C9E58C0634B2F7D26B1F22501DD93FDAE5) |


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

{{< /details >}}
-----



[*source*](https://github.com/magicsword-io/bootloaders/tree/main/yaml/fd70f49d-4efd-4ebb-a889-5dbbcebe33a0.yaml)

*last_updated:* 2023-08-03








{{< /column >}}
{{< /block >}}
