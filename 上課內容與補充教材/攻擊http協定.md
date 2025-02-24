## 網站協定 HTTP vs HTTPS
- HTTP
  - HTTP 1.1
  - HTTP 2(2015年)
  - HTTP 3(2022年6月)
  - Cloudflare的統計，目前最普及的協定仍是HTTP/2，市占率超過60%，HTTP/3市占率則接近30% 
- HTTPS
  - https://www.shubo.io/https/ 


## HTTP 1.1
- HTTP Header Injection
  - https://ithelp.ithome.com.tw/articles/10268595 
- HTTP Request Smuggling
  - https://ithelp.ithome.com.tw/articles/10267371
  - https://www.freebuf.com/articles/web/213360.html
  - [Hiding Wookiees in HTTP](https://media.defcon.org/DEF%20CON%2024/DEF%20CON%2024%20presentations/DEF%20CON%2024%20-%20Regilero-Hiding-Wookiees-In-Http.pdf)
  - [HTTP Desync Attacks: Request Smuggling Reborn | James Kettle](https://portswigger.net/research/http-desync-attacks-request-smuggling-reborn)
  - [HTTP Request Smuggling in 2020–New Variants, New Defenses and New Challenges |Amit Klein](https://i.blackhat.com/USA-20/Wednesday/us-20-Klein-HTTP-Request-Smuggling-In-2020-New-Variants-New-Defenses-And-New-Challenges-wp.pdf)   
- HTTP flood DDoS attack
## HTTP 2
- CVE-2023-44487漏洞
  - [HTTP/2協定漏洞帶來史上最大DDoS攻擊流量，Google、Cloudflare與AWS皆創紀錄](https://www.ithome.com.tw/news/159221)
  - 利用HTTP/2中的多工串流（Stream Multiplexing）功能
  - 發送大量的請求且立即取消，因而造成伺服器端的大量工作負載，卻只需要少量的攻擊成本。
  - 根據估計，駭客針對CVE-2023-44487漏洞展開攻擊時所利用的殭屍網路僅由2萬臺機器組成，遠低於目前動輒由數十或數百萬臺機器組成的殭屍網路。
## HTTP 3
- CVE-2022-30592
  - [HTTP3-attacks (CVE-2022-30592)](https://github.com/efchatz/HTTP3-attacks) 
- NGINX HTTP/3 QUIC vulnerability CVE-2024-24989


## 2024年度十大網站攻擊技術手法一覽
- [2024十大網站攻擊技術公布，臺灣資安專家再度稱霸第一](https://www.ithome.com.tw/news/167513)
- 1. Confusion Attacks: Exploiting Hidden Semantic Ambiguity in Apache HTTP Server  -  Orange Tsai
- 2. SQL Injection Isn't Dead: Smuggling Queries at the Protocol Level - Paul Gerste
- 3. Unveiling TE.0 HTTP Request Smuggling - Paolo Arnolfo、Guillermo Gregorio、 @_medusa_1_
- 4. WorstFit: Unveiling Hidden Transformers in Windows ANSI - Orange Tsai、Splitline
- 5. Exploring the DOMPurify library: Bypasses and Fixes - Mizu
- 6. DoubleClickjacking: A New Era of UI Redressing - Paulos Yibelo
- 7. CVE-2024-4367 - Arbitrary JavaScript execution in PDF.js - Thomas Rinsma
- 8. OAuth Non-Happy Path to ATO - Oxrz
- 9. ChatGPT Account Takeover - Wildcard Web Cache Deception- Harel
- 10. Hijacking OAuth flows via Cookie Tossing - Elliot Ward
