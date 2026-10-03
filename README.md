# Stellar Odyssey Perú — Evaluación de Jurado

Fui jurado en **Stellar Odyssey Perú**, el hackathon de la comunidad de Stellar en Perú, y evalué los 30 proyectos presentados según el rubric oficial del panel. Este repo documenta cómo llegué a cada puntaje: para cada proyecto revisé su repositorio, verifiqué que la evidencia on-chain declarada existiera realmente en testnet, y contrasté eso con la descripción que cada equipo presentó.

**Pesos del rubric:** Funcionalidad/testnet 30% · Integración técnica 25% · Originalidad/track 20% · Viabilidad 15% · Claridad README/video 10%

Los 30 puntajes ya están cargados en el panel oficial del jurado; esto queda como respaldo de mi evaluación.

## Tabla de puntajes

| # | Proyecto | Track | Func (30%) | Integración (25%) | Originalidad (20%) | Viabilidad (15%) | Claridad (10%) | **Total /5** |
|---|---|---|:-:|:-:|:-:|:-:|:-:|:-:|
| 14 | Honorarios | RWA & Compliance | 5 | 5 | 5 | 4 | 4 ⚠ | **4.75** |
| 4 | ArenaPay | Gaming & Physics | 5 | 5 | 5 | 3 | 5 | **4.70** |
| 23 | Pakta | AI Agents | 5 | 5 | 5 | 4 | 3 🎥 | **4.65** |
| 6 | CanguPAY | AI Agents | 5 | 5 | 4 | 5 | 3 🎥 | **4.60** |
| 24 | Paul | RWA & Compliance | 5 | 4 | 5 | 4 | 4 🎥 | **4.50** |
| 20 | NikoSun | RWA & Compliance | 5 | 4 | 5 | 4 | 3 🎥 | **4.40** |
| 8 | CrimsonSentry | Research & Crypto | 4 | 5 | 5 | 4 | 3 🎥 | **4.35** |
| 10 | Eco Bonus | Gaming & Physics | 5 | 5 | 3 | 4 | 3 🎥 | **4.25** |
| 16 | Masi | Open Build | 5 | 5 | 3 | 4 | 2 📉🎥 | **4.15** |
| 3 | AgreedPay | RWA & Compliance | 5 | 4 | 3 | 4 | 4 | **4.10** |
| 17 | MergePay | AI Agents | 5 | 4 | 4 | 3 | 3 🎥 | **4.05** |
| 9 | DeRaíz | RWA & Compliance | 4 | 4 | 4 | 4 | 4 | **4.00** |
| 29 | Vera | Realtime Finance | 4 | 4 | 4 | 4 | 3 📉 | **3.90** |
| 2 | AgenteKipu | AI Agents | 4 | 3 | 5 | 4 | 3 🎥 | **3.85** |
| 7 | Chocolatito | AI Agents | 5 | 2 | 5 | 3 | 4 🎥 | **3.85** |
| 21 | OSS 402 | AI Agents | 3 | 5 | 5 | 3 | 1 📉🎥 | **3.70** |
| 30 | VoxPay | Open Build | 4 | 4 | 4 | 4 | 1 📉🎥 | **3.70** |
| 1 | Aegis | AI Agents | 4 | 3 | 4 | 4 | 3 🎥 | **3.65** |
| 18 | Minka Capital | Realtime Finance | 4 | 3 ⚠ | 4 | 3 | 4 | **3.60** |
| 5 | Ayni | Open Build | 4 | 3 | 4 | 4 | 2 📉🎥 | **3.55** |
| 25 | PULS3 | AI Agents | 2 ⚠ | 5 | 5 | 4 | 1 📉🎥 | **3.55** |
| 11 | Escala | Open Build | 4 | 3 | 4 | 4 | 1 📉🎥 | **3.45** |
| 12 | EscudoPay | Research & Crypto | 3 | 3 | 5 | 3 | 3 🎥 | **3.40** |
| 26 | Qhapaq | RWA & Compliance | 4 | 3 | 3 | 3 | 4 | **3.40** |
| 13 | Hito | Open Build | 3 | 4 | 4 | 3 | 2 📉 | **3.35** |
| 27 | Stellar Rail | RWA & Compliance | 3 | 3 | 4 | 4 | 3 ⚠ | **3.35** |
| 28 | StellarYield AI | AI Agents | 4 | 4 | 3 | 3 | 1 📉🎥 | **3.35** |
| 15 | LocalLoop | Open Build | 4 | 3 | 3 | 3 | 1 📉🎥 | **3.10** |
| 19 | Naru | AI Agents | 4 | 2 ⚠ | 3 | 3 | 1 📉🎥 | **2.85** |
| 22 | PagaJusto | AI Agents | 3 | 3 | 2 | 3 | 1 📉🎥 | **2.60** |

⚠ = ver hallazgo en la tabla de integración técnica. 📉 = Claridad bajada por README corto. 🎥 = Claridad bajada (o ya en piso) tras mirar el video demo real.

**Criterio de palabras de README (parte del puntaje de Claridad):** ≤700 → 1 · 700–1000 → 2 · 1000–1500 → 3 · 1500–2500 → 4 · >2500 → 5 (salvo flags de links duplicados o rotos, que bajan el puntaje aparte). Cayeron por este criterio: OSS 402 (428 palabras), StellarYield AI (663), VoxPay (784), PULS3 (890), Naru (945), Escala (998), LocalLoop (1044), Hito (1152), Vera (1246), Ayni (1274), Masi (1300).

## Detalle de integración técnica con Stellar

| # | Proyecto | Tipo de integración | Detalle |
|---|---|---|---|
| 1 | Aegis | Clásico | Agente firma pagos con `stellar-sdk` (JS), sin contrato Soroban. Docs mencionan exploración de x402/Soroban, no implementada. |
| 2 | AgenteKipu | Clásico | `stellar_sdk` (Python) contra Horizon Testnet, pago nativo firmado por el agente sin intervención humana. |
| 3 | AgreedPay | Soroban | Contrato `escrow_milestones` (Rust, con `test.rs`) + SAC USDC + transacciones patrocinadas (sin gas). |
| 4 | ArenaPay | Soroban | Contrato `arena_escrow` (Rust) custodiando inscripciones; Freighter firma depósito; replay verificable off-chain. |
| 5 | Ayni | Clásico | Custodia vía bóveda virtual (trustline/claimable balance); tests reales contra testnet (`verify.test.ts`, `live.test.ts`). |
| 6 | CanguPAY | Soroban | Contratos `conditional-payment` + `test-token` + servicio de attestation (Rust), deploy con Docker. |
| 7 | Chocolatito | Clásico | USDC (SAC) por tarea, firma local del agente, sin contrato custom y sin tests. |
| 8 | CrimsonSentry | Soroban | Contrato `policy-vault` (soroban-sdk 28) con `require_auth` y reglas de gasto acotado. |
| 9 | DeRaíz | Clásico (avanzado) | Activo clásico emitido con `AUTH_REQUIRED` + `AUTH_REVOCABLE` + `AUTH_CLAWBACK_ENABLED` — compliance impuesto por la red. |
| 10 | Eco Bonus | Soroban | 3 contratos: `mission-contract`, `certificate-nft`, `reward-contract`. |
| 11 | Escala | Clásico + terceros | Usa Trustless Work (SDK de escrow de terceros) sobre Stellar + Cavos (login social/smart wallet). |
| 12 | EscudoPay | Clásico | Cuenta con condición de liberación; backend NestJS + `stellar-client` propio. |
| 13 | Hito | Soroban | Contrato `hito-escrow`: acuerdos comprometidos por hash, roles pagador/proveedor separados. |
| 14 | Honorarios | Soroban | Contrato `split`: retención automática del 8% en la misma transacción de cobro. "Abrir video" y "Video pitch" apuntan al mismo link (mismo caso que Stellar Rail). |
| 15 | LocalLoop | Clásico | USDC vía SDK clásico + servidor MCP propio para exponerlo a agentes de IA. |
| 16 | Masi | Soroban | Contrato `escrow` + passkeys/smart account (cuenta abstracta), 56 archivos de test (el más testeado). |
| 17 | MergePay | Soroban | Contrato `escrow` ligado a verificación de Pull Requests de GitHub. |
| 18 | Minka Capital | Soroban (parcial) ⚠ | Contrato propio `minka-market`, mezclado con contratos de scaffold genérico sin usar (`nft-enumerable`, `fungible-allowlist`, `guess-the-number`) que inflan el conteo sin aportar lógica de negocio. |
| 19 | Naru | Soroban (boilerplate) ⚠ | Los contratos presentes (`nft-enumerable`, `fungible-allowlist`) son de scaffold genérico; no se observa lógica de negocio propia de "Naru". |
| 20 | NikoSun | Soroban | Contrato `niko_project` para tokenización RWA de activos de energía limpia. |
| 21 | OSS 402 | Soroban + x402 | Contrato `oss402-attestation` ligado al protocolo de pagos HTTP x402. |
| 22 | PagaJusto | Soroban | Contrato `escrow` con tests, pero solo 5 commits — muy poca iteración. |
| 23 | Pakta | Soroban | Contrato `payable-contract`: valida factura/orden/wallet antes de autorizar el pago. 55 archivos de test. |
| 24 | Paul | Soroban | Contrato `soroban-pool` (tramos senior/junior); 12 instancias desplegadas según la descripción, pero solo 1 archivo de contrato pese a specs extensas — posible brecha entre documentación e implementación. |
| 25 | PULS3 | Soroban | Contratos `identity-registry` (estilo ERC-8004) + `escrow`. Evidencia on-chain rota: el link es un contract ID inválido (16 caracteres en vez de 56). |
| 26 | Qhapaq | Clásico | Activos de participación clásicos (`lib/stellar/*`) + evidencias almacenadas en IPFS. |
| 27 | Stellar Rail | Clásico | Motor de reglas propio corre off-chain (`lib/riel`); el cumplimiento no está impuesto directamente por la red. "Abrir video" y "Video pitch" apuntan al mismo link. |
| 28 | StellarYield AI | Soroban | Contrato `stellaryield-vault` (vault de estrategias de rendimiento), con tests. |
| 29 | Vera | Soroban | Contrato `spending_vault` (tesorería, reembolsos automatizados), con tests. |
| 30 | VoxPay | Soroban | Contrato `voxpay`: reparto atómico de pago en una sola transacción. |

## Links por proyecto

El video demo de cada proyecto fue revisado para definir el puntaje de Claridad. Cuando hay inconsistencias entre demo y pitch (por ejemplo, apuntando al mismo video), lo marco.

| # | Proyecto | Repo | App | Evidencia on-chain | Video demo | Video pitch |
|---|---|---|---|---|---|---|
| 1 | Aegis | [repo](https://github.com/Seb0401/Aegis) | — | [tx](https://stellar.expert/explorer/testnet/tx/d379a163e28c801977da80e683286624507cadfc8354435e88d199fbd0b2e146) | [demo](https://youtu.be/O7Tt1Bbwo9Y) | [pitch](https://www.youtube.com/watch?v=vBH8Z8BJE1c) |
| 2 | AgenteKipu | [repo](https://github.com/luislinodev/AgenteKipu) | — | [tx](https://stellar.expert/explorer/testnet/tx/9ea8404af7f07a4b3514bd60c5d49b894ca240e278217de13267f21828d9be51) | [demo](https://www.youtube.com/watch?v=69QvW5GPcb0) | [pitch](https://youtu.be/wfrtcOXkyQo) |
| 3 | AgreedPay | [repo](https://github.com/elizacl/AgreedPay) | [app](https://agreedpay.vercel.app/) | [contract](https://stellar.expert/explorer/testnet/contract/CCS46B4ENVJLAKUVGPIUZOLL4YLLAP5ZGCSTOGDFEAAYM6IRN5FD24DN) | [demo](https://youtu.be/HJeKQ3DQliQ) | [pitch](https://youtu.be/7s1Gv0zuRFc) |
| 4 | ArenaPay | [repo](https://github.com/hvaler/ArenaPay) | [app](https://arenapay.vercel.app/) | [tx](https://stellar.expert/explorer/testnet/tx/b8f1d444402c4bcb976126b8e144eabde40b6e5dc8fb173f0a63ed178e43b448) | [demo](https://youtu.be/LECz_vXmFi0) | [pitch](https://youtu.be/4uiet8NSKwo) |
| 5 | Ayni | [repo](https://github.com/alexandra585/Ayni) | [app](https://ayni-ten.vercel.app/) | [tx](https://stellar.expert/explorer/testnet/tx/6fcfe0961a0f06528437200618cc53e00add122a3d6e0a47cec189752f134c38) | [demo (drive)](https://drive.google.com/drive/folders/1Ty_pXBr3NcydPDIuE2S1__uBn10gJIXt) | [pitch](https://youtu.be/aOUFziSK4Yo) |
| 6 | CanguPAY | [repo](https://github.com/gonnnzaDev/CanguPay) | [app](https://cangupay.vercel.app/landing) | [tx](https://stellar.expert/explorer/testnet/tx/f7168ae3e3c0f4e7cf59bc66353f7d9f3e24510043144dcf4864b2f003e1976f) | [demo (drive)](https://drive.google.com/drive/folders/1XsBEdXInQ2g-YM-DOHJ4LRQWdiPpOoXS) | [pitch](https://youtu.be/Su-RGzgh5hw) |
| 7 | Chocolatito | [repo](https://github.com/chocolatito27/chocolatito-stellar) | [app](https://chocolatito.space/) | [tx](https://stellar.expert/explorer/testnet/tx/a0c3956d497101e66ea731e16a4320468b9f62ca4dfa860f69bda31ec13a947c) | [demo](https://youtu.be/xIyeMhX-L9A) | [pitch](https://youtu.be/OlzHY2O3m6s) |
| 8 | CrimsonSentry | [repo](https://github.com/JoseEscajadillo/CrimsonSentry) | — | [contract](https://stellar.expert/explorer/testnet/contract/CB5X32K4QZLPO6YZYE2KWZW2QAXXUT5AJSJJFF2OP73IYCFMCYZJEBXG) | [demo](https://youtu.be/lgQYx48JnV0) | [pitch](https://youtu.be/Lhr5abKy-eI) |
| 9 | DeRaíz | [repo](https://github.com/diegoortizcpn-svg/deraiz) | [app](https://deraiz.lovable.app/) | [tx](https://stellar.expert/explorer/testnet/tx/a8d76860ff91c2636e8d329bc761099201661e8418760fc3806da91ddbe7ddcc) | [demo](https://www.youtube.com/watch?v=gpWHHc6ZjRI) | [pitch](https://www.youtube.com/watch?v=wOVxvtTs9FM) |
| 10 | Eco Bonus | [repo](https://github.com/carlos-israelj/EcoBonus) | [app](https://carlos-israelj.github.io/EcoBonus/login) | [contract](https://stellar.expert/explorer/testnet/contract/CBITQYMLPOOOHZ3EXYKQFKB7XMOOLXIWH5WKTU6DAKZAJ5WFR5SFKUZK) | [demo](https://youtu.be/mk7VHQghpYk) | [pitch (drive)](https://drive.google.com/drive/folders/1o7jN6YADpPl9DiAhnC5p68oUHjWvDAJ9) |
| 11 | Escala | [repo](https://github.com/salazarsebas/escala) | [app](https://escala.acachete.xyz/) | [tx (acachete)](https://stellarview.acachete.xyz/es/testnet/tx/1783def018811b729092fada479b724637d49c117f305a818356239a3a018671) | [demo](https://youtu.be/iPg-G95T0Yo) | [pitch](https://youtu.be/bmZMx_i8Yb8) |
| 12 | EscudoPay | [repo](https://github.com/Mei001x/EscudoPay) | [app](https://shieldpay.caychopomachagua.dev/) | [tx](https://stellar.expert/explorer/testnet/tx/21e3b167dcee38429d7963a676c9adbd758a6f02acf2d4dc94f21ddd62124444) | [demo](https://youtu.be/vZQE1Z-SsMA) | [pitch](https://youtu.be/iNjsDmAxdag) |
| 13 | Hito | [repo](https://github.com/NyroCode/hito-agent-native) | — | [tx](https://stellar.expert/explorer/testnet/tx/1ff3b0c2ff51723cac49d8044ce0e3e7fbe44e9cc51f57c77fbb8eaec6c1e080) | [demo (drive)](https://drive.google.com/file/d/1WtUUXiClsKV-QfUmRW99R_xnJ13e-qdV) | [pitch (drive)](https://drive.google.com/file/d/1Fe9wDq9jbKIBzNQ7hdFbroFllu_MDopd) |
| 14 | Honorarios | [repo](https://github.com/kasbsquall/honorarios) | [app](https://honorarios-pe.vercel.app/) | [contract](https://stellar.expert/explorer/testnet/contract/CAWIYCJAOXFIL5XHIIXK34XOSLSFTLUU5LP6JEL65QECGZM5WATUXDDF) | [demo](https://youtu.be/L0_wNoNNIJ0) | [pitch — mismo link que demo](https://youtu.be/L0_wNoNNIJ0) |
| 15 | LocalLoop | [repo](https://github.com/GonzaloRail/LocalLoop) | [app](https://localloop-zeta.vercel.app/) | [tx](https://stellar.expert/explorer/testnet/tx/6b5286a7a5a820f7f25b3e0874f355c185cf3ebfbce2b60c7cbb81f4b4d4e5ab) | [demo](https://youtu.be/tu_VofGc9-s) | [pitch](https://youtu.be/C8pjITF7zVE) |
| 16 | Masi | [repo](https://github.com/piales00/masi) | [app](https://masiapp.vercel.app/) | [contract](https://stellar.expert/explorer/testnet/contract/CAGC224PARRU3DZOCRUKOPCFGJU2ADOTNVETMDROKVT6QA5KYXBZ2DVL) | [demo](https://youtu.be/-NJoaORmGWQ) | [pitch](https://youtu.be/_EprX5tx2zI) |
| 17 | MergePay | [repo](https://github.com/CodyLionVivo/mergepay) | [app](https://mergepay-taupe.vercel.app/) | [contract](https://stellar.expert/explorer/testnet/contract/CDNQOP6P3EHO4OBREYQY5ZNQUF2ZY7BNBP7F6MBOEAMJBGK66CDOH5HG) | [demo](https://youtu.be/NB86FQNUc6M) | [pitch](https://youtu.be/IECzusRU0lY) |
| 18 | Minka Capital | [repo](https://github.com/giano-montano/minka-capital) | [app](https://minka-capital.a20212540.workers.dev/) | [tx](https://stellar.expert/explorer/testnet/tx/a1d2200f2506995b199bfffb1dc04df0ab8bad6a5424bce70b14465d9a056eb3) | [demo](https://youtu.be/qkSqF7uODSg) | [pitch](https://youtu.be/I_jE6NKMaFk) |
| 19 | Naru | [repo](https://github.com/mavix21/naru) | [app](https://naru-app-kappa.vercel.app/) | [tx](https://stellar.expert/explorer/testnet/tx/ff7b48c2246124b370cf767e81a7a9a2eea55f1d4730892eb8db35d1ce7aa44e) | [demo](https://youtu.be/T3Sl3tSe1pg) | [pitch](https://youtu.be/3jpPjH41-b4) |
| 20 | NikoSun | [repo](https://github.com/ECOMAM/stellar-energy-assets) | [app](https://niko-sun.netlify.app/) | [contract](https://stellar.expert/explorer/testnet/contract/CAW37S6RDQCRCHUBMFG4KMMZHSNI6AD5AR5MG5OQS76J7FU7JUDR3UAK) | [demo](https://youtu.be/YG9HuD4g3BY) | [pitch](https://youtu.be/fPTjrH5sjfY) |
| 21 | OSS 402 | [repo](https://github.com/hallzyx/oss402) | — | [contract](https://stellar.expert/explorer/testnet/contract/CAHOYKJPZNQ73XH3WCW7KLKWYT3SIHWL3UNEVTDNIMRQPIQMYBAVBMSI) | [demo](https://youtu.be/L6CFM6sHI8M) | [pitch](https://youtu.be/XRfl8VB6z0U) |
| 22 | PagaJusto | [repo](https://github.com/vizarreta/PAGA-JUSTO-) | — | [contract](https://stellar.expert/explorer/testnet/contract/CCYTNDYEETWXBB5NO6CVQEC75FPESVZUS667OR4GHLCQURFXVUV7E665) | [demo (drive)](https://drive.google.com/file/d/1mytWnkeNR0r0bnhREy-AuIKfk04AtgoO) | [pitch (drive)](https://drive.google.com/file/d/1P3zkA6VR-lqYQlWlMVn2CDEwl25KoWNP) |
| 23 | Pakta | [repo](https://github.com/devmondoss/pakta) | [app](https://pakta-eight.vercel.app/) | [contract](https://stellar.expert/explorer/testnet/contract/CBTQDZBJYL2JFQAT64OZYFK4PFOA3EG7CMVZ44FCBSAPDE5EXMTACS6S) | [demo (drive)](https://drive.google.com/drive/folders/110y7b90jJ7O5jyv8A-bZhrKmdV89-tt_) | [pitch](https://youtu.be/jis4zjk3IkI) |
| 24 | Paul | [repo](https://github.com/nicolasIsmael/paul) | [app](https://paul-neon.vercel.app/acceso) | [contract](https://stellar.expert/explorer/testnet/contract/CCGH3FI2775BI2KPA5HDTTRBSTSACE2X2H4ZJJ56NWGUBWQ2NWFGQBWO) | [demo](https://youtu.be/dt_c0VN8DJI) | [pitch](https://youtu.be/AWmY0XNfu6c) |
| 25 | PULS3 | [repo](https://github.com/Zer0-Knowledge-Hack/puls3) | [app](https://puls3-4lw.pages.dev/) | [contract — ID inválido](https://stellar.expert/explorer/testnet/contract/CD5QZOKGRBV35C5S) | [demo (short)](https://youtube.com/shorts/Kd_YgMgMnZ4) | [pitch](https://youtu.be/bcCVxI5_6Ec) |
| 26 | Qhapaq | [repo](https://github.com/gianellacoronel/qhapaq) | [app](https://qhapaq-kappa.vercel.app/es) | [tx](https://stellar.expert/explorer/testnet/tx/43070e06f0ae006e5ebc3357f06d15690cf83087438b5d143a8d2bd895061924) | [demo](https://youtu.be/c_OLRaK8dcQ) | [pitch](https://youtu.be/sQ5svx05j3Y) |
| 27 | Stellar Rail | [repo](https://github.com/Pdelacruz123/stellar-rail) | [app](https://stellar-rail.vercel.app/) | [tx](https://stellar.expert/explorer/testnet/tx/2b2a5be5dec2506408eca90d34233054f675eba1bc4389811dff8730d4d1248d) | [demo](https://youtu.be/F2Qs4IY3r-M) | [pitch — mismo link que demo](https://youtu.be/F2Qs4IY3r-M) |
| 28 | StellarYield AI | [repo](https://github.com/YisusCode1/stellaryield-ai) | [app](https://stellaryield-ai-web.vercel.app/) | [contract (lab.stellar.org)](https://lab.stellar.org/smart-contracts/contract-explorer?%24=network%24id=testnet&smartContracts%24explorer%24contractId=CA23V5M6O6DONEXJWZLYGM3CARXDXNL7HEBOTW7WKE7RLRZK7AF5BQQJ) | — | [pitch](https://youtu.be/FL_tt8IHy0g) |
| 29 | Vera | [repo](https://github.com/angelespinoza/vera) | [app](https://vera-production-5a47.up.railway.app/dashboard) | [contract](https://stellar.expert/explorer/testnet/contract/CDYOVSKH5ABN62NWWTFTSPLKZVBWOODM6XLUVMHLCALNM7JSLPBBTOGY) | [demo](https://youtu.be/mUzt3cczGlM) | [pitch](https://youtu.be/N1wouAVfmB0) |
| 30 | VoxPay | [repo](https://github.com/Rondnt/VoxPay-Stellar) | [app](https://voxpay--voxpay-gj.us-central1.hosted.app/) | [contract](https://stellar.expert/explorer/testnet/contract/CBFO53O3IHNMHCPAGJZXZMN2SOHA3BRKAJHAIRVNFKPZZD4E44BNX57Q) | [demo (drive)](https://drive.google.com/file/d/1M1ciK-tnhu0TS04wT9oswxMDUQXd5L4N) | [pitch (drive)](https://drive.google.com/file/d/1DlBD0HVUtXlhkL5CHIh59Y580Ts3Somp) |

## Metodología

- Extraje los entregables directamente del panel de jurado (descripción, problema que resuelven, cómo usan Stellar, links).
- Cloné cada repo (`git clone --depth 100`) y revisé README, historial de commits, señales de uso de `stellar-sdk`/`soroban-sdk`, archivos de contrato en Rust y archivos de test.
- Verifiqué cada link de evidencia on-chain contra la API pública `api.stellar.expert/explorer/testnet/{tx|contract}/...` para confirmar que la transacción o el contrato existen realmente en testnet.
- Miré el video demo de cada proyecto y ajusté el puntaje de Claridad cuando encontré videos sin audio, demasiado largos (6+ min) o mal editados/confusos.
- Con esa base, puntué los 5 criterios del rubric oficial y dejé feedback puntual a cada equipo.
