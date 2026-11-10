# T02 — Exercicis de classe (resolts)

---

## EC2.1 IT o OT? (b)

| # | Sistema | Classificació | 
|---|---------|:---:|
| 1 | Servidor de correu corporatiu (Microsoft 365) | **IT** |
| 2 | SCADA d'una planta química (vàlvules i sensors) | **OT** | 
| 3 | ERP al núvol (comandes i facturació) | **IT** |
| 4 | PLC que governa una cadena de muntatge | **OT** | 
| 5 | Plataforma de tiquets de suport (Jira, Zendesk) | **IT** | 
| 6 | Sistema MES que connecta el PLC amb l'ERP | **Mix IT/OT** |
| 7 | Programari de còpies de seguretat dels servidors | **IT** | 
| 8 | Control d'accessos d'un edifici (targetes) | **Mix IT/OT** |

---

## EC2.2 Departaments IT d'una empresa (b)

| Àrea / Departament | Què gestiona? | Per què és entorn IT? |
|---|---|---|
| Sistemes i infraestructura | Servidors, xarxa, núvol, còpies de seguretat, comptes d'usuari | Tot són recursos per emmagatzemar, processar i transmetre informació. |
| Desenvolupament de programari | Aplicacions web/mòbil, repositoris de codi, entorns de proves i producció | Crea i manté programari que tracta dades de negoci. |
| Suport tècnic / Helpdesk | Incidències d'usuaris i clients, eina de tiquets, inventari d'equips | Dona servei sobre equips i aplicacions informàtiques. |
| Ciberseguretat | Polítiques d'accés, antivirus/EDR, tallafocs, auditories, RGPD | Protegeix la confidencialitat, integritat i disponibilitat de la informació. |
| Dades i BI | Bases de dades, informes, quadres de comandament | Transforma dades en informació per prendre decisions. |
| Administració / Comercial (usuaris IT) | ERP, CRM, facturació, correu | Usen sistemes d'informació per a tasques de negoci, no per controlar processos físics. |

---

## EC2.3 Tecnologia de negoci vs. de planta (b)

| Tecnologia | Negoci | Planta |
|---|:---:|:---:|
| ERP (SAP, Oracle, etc.) | ✗ | |
| SCADA / HMI | | ✗ |
| CRM (Salesforce, HubSpot) | ✗ | |
| MES (Manufacturing Execution System) | | ✗ |
| E-commerce (PrestaShop, Shopify) | ✗ | |
| PLC / PAC | | ✗ |
| BI / Data Warehouse | ✗ | |
| Robots col·laboratius (cobots) | | ✗ |

---

## EC2.4 Què fa que IT i OT s'assemblin i es diferenciïn (m)

| Aspecte | IT | OT |
|---|---|---|
| **Coincidència 1** — Base tecnològica | Ordinadors, programari i xarxes (Ethernet, TCP/IP). | Cada cop més basada també en equips programables i xarxes IP. |
| **Coincidència 2** — Necessitat de seguretat | Ha de protegir-se de malware, accessos no autoritzats, etc. | També és objectiu d'atacs i necessita mesures de ciberseguretat. |
| **Coincidència 3** — Generen i usen dades | Dades de clients, vendes, gestió… | Dades de sensors, producció, consums… que es poden analitzar. |
| **Diferència 1** — Finalitat | Gestionar informació i suportar processos de negoci. | Controlar i supervisar processos i màquines físiques. |
| **Diferència 2** — Prioritat de seguretat | Primer la confidencialitat de les dades. | Primer la disponibilitat i la seguretat de les persones (una aturada o error pot ser perillós). |
| **Diferència 3** — Cicle de vida i actualitzacions | Equips renovats cada 3-5 anys; pegats freqüents i fàcils d'aplicar. | Equips que duren 15-30 anys; actualitzar implica aturar producció, per això es pegueja poc. |

---

## EC2.5 Convergència IT-OT d'una consultora IT (m) — BIT Consultors

**1. Entorn IT i entorn OT**
- **IT de BIT Consultors:** la seva infraestructura pròpia — plataforma al núvol, servidors, xarxa corporativa, eines de monitorització, ticketing, correu, ERP/CRM i els equips dels tècnics.
- **OT del client:** la línia de producció, la climatització i les instal·lacions físiques (i la seva sala de servidors com a infraestructura física: temperatura, energia) on es col·loquen els sensors IoT.

**2. Sistema pont**
La **plataforma al núvol de monitorització** juntament amb els **sensors/gateways IoT**: recullen dades del món físic (OT) i les porten al sistema informàtic de BIT (IT).

**3. Tecnologia habilitadora**
L'**IoT industrial (IIoT)** combinat amb el **cloud computing** i la connectivitat (Internet, 4G/5G, VPN). Els sensors envien dades en temps real al núvol i el tècnic les consulta des de qualsevol lloc amb un panell web.

**4. Avantatges per al client industrial**
- Manteniment **preventiu/predictiu**: es detecten anomalies abans que la màquina falli.
- Menys **aturades no planificades** i menys costos de reparació.
- No cal tenir personal especialitzat propi ni desplaçaments de tècnics.
- Històric de dades per prendre decisions (consums, rendiment, eficiència energètica).

**5. Risc nou**
La instal·lació industrial, abans aïllada, ara està **connectada a Internet**: apareix una nova **superfície d'atac**. Un atacant podria entrar pels sensors o la plataforma i arribar a la xarxa OT, provocant aturades, manipulació de dades o danys físics. També hi ha dependència de la connexió i del proveïdor.

---

## EC2.6 Avantatges d'una digitalització d'extrem a extrem (m) — DeltaCode

| Àmbit | Avantatge | Justificació (1-2 frases) |
|---|---|---|
| **Dades / Integració** | Informació única i actualitzada del sensor al client | El MES envia les dades de la maquinària directament al SaaS d'inventari, sense introduccions manuals ni errors de còpia. |
| **Operativa** | Inventari en temps real | Les pimes saben l'estoc exacte en cada moment i poden reaccionar abans de quedar-se sense material. |
| **Servei al client** | Suport 24×7 proactiu | El NOC detecta incidències abans que el client se n'adoni i les resol ràpidament, cosa que millora la satisfacció. |
| **Model de negoci** | Ingressos recurrents i escalables | Passar de vendre hores a una subscripció SaaS dona ingressos estables i permet atendre molts clients amb el mateix producte. |
| **Presa de decisions** | Analítica sobre tota la cadena | Tenint dades des de producció fins a l'ús del client es poden detectar patrons, predir demanda i optimitzar processos. |
| **Costos** | Menys feina manual i menys errors | L'automatització redueix temps de gestió i costos derivats d'errors humans. |

---

## EC2.7 Riscos de connectar OT a Internet (r) — Planta de packaging

| # | Risc | Tipus | Mesura de mitigació |
|---|---|---|---|
| 1 | **Accés no autoritzat al SCADA** (atacants que el troben exposat a Internet amb eines com Shodan) | Seguretat | No exposar-lo directament: accés remot només per **VPN** amb **autenticació multifactor (MFA)** i comptes individuals. |
| 2 | **Malware / ransomware** que entra per la connexió i atura la producció | Seguretat / operacional | **Segmentació de xarxa** (model Purdue, DMZ industrial) amb **tallafocs** entre IT, Internet i OT; antimalware compatible i llistes blanques d'aplicacions. |
| 3 | **Programari antic sense pegats** (SCADA/HMI amb vulnerabilitats conegudes) | Tècnic | Inventari d'actius, **gestió de vulnerabilitats** i aplicar pegats en finestres de manteniment planificades; si no es pot, controls compensatoris (aïllament, IPS industrial). |
| 4 | **Credencials febles o compartides** amb el proveïdor (contrasenyes per defecte) | Seguretat | Canviar contrasenyes per defecte, principi de **mínim privilegi**, accés del proveïdor **temporal i sota demanda**, i **registre/gravació de sessions**. |
| 5 | **Manipulació de processos** (canvi de paràmetres de màquines) que causa danys físics o productes defectuosos | Operacional / safety | Accés del proveïdor **només de lectura** per defecte; canvis amb aprovació interna; sistemes de seguretat (SIS) independents i aïllats. |
| 6 | **Pèrdua de connexió o latència** que afecta el control | Tècnic / operacional | El control crític ha de funcionar **en local** sense dependre d'Internet; connexió redundant i monitorització. |
| 7 | **Manca de visibilitat** sobre què fa el proveïdor | Seguretat | **Monitorització i logs** del tràfic OT (IDS industrial), auditories periòdiques i contracte amb requisits de seguretat (p. ex. IEC 62443). |