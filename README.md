# Queries for hunting exposed C2 panels using Urlscan.io

### Reader`s Notes

This repo contains a series of search queries one could use to run and hunt for exposed C2 panels and adversary infrastructure . The searches are mainly based on searching for C2 panels through page titles , favicon hashes and page hashes

All of these searches could be run directly through the Urlscan.io`s search tab at :- https://urlscan.io/search/#*

### Acknowledgements 

Most of these queries were based on the incredible work by [MichalKoczwara](https://x.com/MichalKoczwara) and [Viriback](https://viriback.com/author/admin-vb/)

<details>
<summary><h4 style="display:inline"> Super Shell Search Query </h4></summary>

```
page.url:"supershell/login/*"

```
</details>

<details>
<summary><h4 style="display:inline"> Caldera C2 </h4></summary>

```
page.title:"Login | CALDERA"
```

</details>

<details>
<summary><h4 style="display:inline"> Chaos Control Panel </h4></summary>

```
hash:b78ec7d301f2d25c974800c136c583b7b5a25ec5ec13dbf04cae9817fa8045aa

Additional search way :- any URL with the href "https://github.com/tiagorlampert/CHAOS"
```

</details>

<details>
<summary><h4 style="display:inline"> Unam Control Panels </h4></summary>

```
page.title:"Unam Web Panel"
```

</details>

<details>
<summary><h4 style="display:inline"> Metasploit Panel </h4></summary>

```
page.title:"Metasploit" AND hash:18fa5b7a32e5528d71a1b9a0544d1f12ad242293e5be2177d08b43cd8a23e343
```

</details>

<details>
<summary><h4 style="display:inline"> Mythic Malware </h4></summary>

```
hash:b32e353c931680b708ab19df96d01ed3c2dc755f210c3934bac899b58a4865e7 AND page.title:"Mythic"
```

</details>

<details>
<summary> <h4 style = "display:inline"> Gophish Login Terminals </h4> </summary>
 
```
page.title:"Gophish - Login"  OR hash:6f383235d8dec5350c1233c04b035b116bbbd2b287c13deb298a123dc5e49d03
```

</details>

<details> 
<summary> <h4 style = "display:inline">Meduza Stealer </h4> </summary>

```
page.title:"Meduza Stealer" AND hash:8f7b512b0e33917c7309ed4a2e9b0ac646a9fb64505b80e8a2dc715185cf855b
```
</details>

<details> 
<summary> <h4 style = "display:inline"> Hookbot Panels </h4> </summary>

```
page.title:"Hookbot Panel" OR hash:b26651525e75ecd609b482e0d3dfad4cbc6e86670e73d06a787be342b042e877

```
</details>

<details>

<summary> <h4 style = "display:inline"> Blacknet Botnet </h4> </summary>

```
page.title:"BlackNet - Login" OR hash:f2d021a4d90fac7a00c51d2695e5e806822a1c07d62eb001921cb5659c77cb1f OR hash:35981130af78c4c56e635745e90abeb45dfd30d83364e62b0557b4af76d75fdd
```

</details>

<details> 

<summary> <h4 style = "display:inline"> Spectre Stealer </h4> </summary>


```
page.title:"'Spectre Stealer - Login" OR hash:7025c9eb6bce3afd5d5290b1b71bd9e77c111740958516401b1e622b9d7d56c0

```
</details>

<details>
<summary> <h4 style = "display:inline"> Prysmax Stealer </h4> </summary>

```
page.title:"'Prysmax Stealer"
```
</details>

<details>

<summary> <h4 style = "display:inline"> Mobile Security Framework </h4> </summary>

```
page.title:"'Mobile Security Framework - MobSF" OR hash:49d4c44292ffe6c30273d925e86377837c9236bf1d8c1dd1bad61fcde50edf1f
```

</details>

<details>

<summary> <h4 style = "display:inline"> Vshell - 登录 </h4> </summary>

```
page.title:"Vshell - 登录" OR hash:"b174afa4328da74bab702857c9e1a0c072cf9e04ab2ba232ee997bdcaa264ee1"

```

</details>

<details>

<summary> <h4 style = "display:inline"> PoshC2 </h4> </summary>

```
hash:fe7e5b2b5df251e256a581eb321b3f3d28f0f3a7031811d60ee0b9f1560fc374
```

</details>

<details>

<summary> <h4 style = "display:inline">  Gotham Stealer </h4> </summary>

```
page.title:"Gotham Stealer" OR hash:4b2495d41f1a96212b03a7d541375378b8cbb136d46353eeaa0110d28d884ab8
```

</details>

<details>

<summary> <h4 style = "display:inline"> Mystic Stealer </h4> </summary>

```
page.title:"Mystic Stealer" OR hash:5eab2b1a633ac3b2148189ed188ee31e71943da8b5cb2928d2ae59046408bd5a
```

</details>

<details>

<summary> <h4 style = "display:inline"> Titan Stealer </h4> </summary>

```
page.title:"Titan Stealer" OR hash:97dc757926a376de09b8628f63342b4ea7b0a652cc7523d35ee9d6f1a98bb0ee
```

</details>

<details>

<summary> <h4 style = "display:inline"> Patriot Stealer </h4> </summary>

```
page.title:"patriot Stealer"
```

</details>

<details>

<summary> <h4 style = "display:inline"> Hak5 Cloud C2 </h4> </summary>

```
hash:e44ede0890d5baf4805a34185e65a28c5cfd53052b080ba72026d69445f636a8 OR  page.title:"Hak5 Cloud C²"
```

</details>

<details>

<summary> <h4 style = "display:inline"> Nimplant C2 </h4> </summary>

```
server:"NimPlant C2 Server"
```

</details>

<details>

<summary> <h4 style = "display:inline"> Deimos C2 </h4> </summary>

```
page.title:"Deimos C2" OR hash:"4bb3ee8361794353b8f76f97778fd377838b1354193b552cad5b3bf742cc9b34"
```

</details>

<details>

<summary> <h4 style = "display:inline"> Covenant C2 </h4> </summary>

```
page.title:"Covenant - Login" OR hash:"96bde84b645282cc37b4326e8b02d04e8b742e70e50a012d405f83eeee872a68"
```

</details>

<details>

<summary> <h4 style = "display:inline"> Amadey </h4> </summary>

```
hash:54713a2d801093e2d318a36f662604649aeb8bd6f649bec00c53abf6813f2014
```

</details>

<details>

<summary> <h4 style = "display:inline"> Overlord </h4> </summary>

```
hash:3f40b48141a3f71d1d7c24adc59622060fc7fb99bbfb54a26eb76060d00278ec

```

</details>

<details>

<summary> <h4 style = "display:inline"> Ghostnet </h4> </summary>

```
hash:7f8b148c4dd80c5d1dbde89a707db5f6ce936d5508837b47b61c23cd15595ad6 OR hash:f0bf30294f5166da1417e959e6e521579b0d116e81b63580d15ac0094ec4c6c1 OR page.title:"GhostNet — Login"
```

</details>

<details>

<summary> <h4 style = "display:inline"> EvilSoul </h4> </summary>

```
hash:b9c23e3513dd38ac8a1b75af54cf7bbbad667f070cfeaca5302a7f3cad32d3ae OR hash:44fcece36915966b7310a648a5acfa8f39985fa7d4253891d0871b59c2b7eea4

```

</details>

<details>

<summary> <h4 style = "display:inline"> XLoader </h4> </summary>

```
hash:205679dec05cf6a7b2903caab9407432eba27341c71161dd1f036a04f02db618 OR page.title:"XL - Login"

```

</details>

<details>

<summary> <h4 style = "display:inline"> Ghostshell </h4> </summary>

```
hash:bcdf194b4e5b1efba0716aa6c25de6130a00bfdc1e7f223311d11d1ba76d24c9 OR page.title:"GhostShell C2" OR hash:"bcdf194b4e5b1efba0716aa6c25de6130a00bfdc1e7f223311d11d1ba76d24c9"
```

</details>

<details>

<summary> <h4 style = "display:inline"> ZShell </h4> </summary>

```
hash:c1cc503e513f803b44bb1b0477fbdfffa4fc68e1fe377becc2114fcf0ae01f62 OR page.title:"Zshell C2 Framework"
```

</details>

<details>

<summary> <h4 style = "display:inline"> 751 </h4> </summary>

```
hash:f62b5a532baeca754ee7fa00c321b2e90ce32dc37e86ad0d9cb01d974e2cee10 OR hash:"751 Stealer |"
```

</details>

<details>

<summary> <h4 style = "display:inline"> PFStealer </h4> </summary>

```
hash:cc33d45cb8247cbbce2a3b35723a9c3e7d70f6275d9656f9f75fdee72a26a90b OR page.title:"PF Stealer - Login"
```
</details>

<details>

<summary> <h4 style = "display:inline"> Lokibot </h4> </summary>

```
page.url:"PvqDq929BSx_A_D_M1n_a.php"

```
</details>

<details>

<summary> <h4 style = "display:inline"> Cyber Aliens </h4> </summary>

```
hash:c735b43a0715bbc07601aa7c208e1ae1381ae745318cd104910a18c66d75563c OR page.title:"Cyber Aliens"
```
</details>

> [!WARNING]
> ### Disclaimers


The queries in this repository are provided for **defensive security, threat intelligence, and research purposes only**. They are intended to help security professionals identify and track malicious infrastructure using publicly available data indexed by [urlscan.io](https://urlscan.io).

- This project does **not** contain, host, or distribute malware, exploits, or live operator credentials.
- Query results reflect third-party scan data and may include false positives, stale entries, or legitimate services. **Validate findings independently** before taking action (blocking, takedown requests, attribution).
- Do not use these queries to access, probe, or interfere with systems you do not own or are not authorized to test. Interacting with discovered hosts may be illegal in your jurisdiction.
- Do not use this repository to facilitate harassment, doxxing, or unauthorized attribution of individuals.
- Use of urlscan.io is subject to its [Terms of Service](https://urlscan.io/about/) and API rate limits.
- The author(s) provide this content **"as is" without warranty of any kind** and accept no liability for misuse, damages, or actions taken based on its contents.
- By using this repository, you agree to use it lawfully and responsibly.
