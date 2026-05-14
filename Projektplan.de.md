# Projekt Firmennetzwerk 2
> **Standortvernetzung über IP-Transit** | 4-Wochen-Projektplan

## 📊 Gesamtübersicht
| Woche | Nataliia (ca. 50%) | Anh (ca. 50%) |
| :--- | :--- | :--- |
| **1** | Topologie, Wien komplett | ISP-Router + Netzdiagramm + Linz Basis |
| **2** | GRE Tunnel HQ + NAT/PAT | GRE Branch + Graz komplett |
| **3** | ACL File-Server + Security-Doku | Port Security + Inter-Site Tests |
| **4** | Review + Abschlusstests | Bandbreite + Dokumentation + PT-Cleanup |

---

## 📅 Woche 1: Grundkonfiguration & ISP
### Nataliia
- [x] Topologie (Anordnung der Netzwerkgeräte) definiert und verkabelt
- [x] IP-Schema / VLSM (Variable Length Subnet Masking) berechnet
- [x] Transit-Netze und GRE-Tunnel-Netze (/30) berechnet
- [x] VLAN-Schema erstellt (VLAN 10/20/30)
- [x] WEB-Server konfiguriert (Statische IP, HTTP Dienst)
- [x] HQ-Wien-Router: Router-on-a-Stick (Subinterfaces für VLANs) konfiguriert
- [x] DHCP Pools für Wien erstellt

### Anh
- [ ] Netzdiagramm (Grafische Darstellung des Netzwerks) finalisieren
- [ ] ISP-Router: Schnittstellen konfigurieren (Gi0/0, Gi0/1, Gi0/2)
- [ ] Branch-Linz-Router: Basis-Konfiguration & DHCP Pool
- [ ] Switch2 (Linz): VLAN Access-Ports und Uplink
- [ ] Ping-Tests: ISP zu allen Standorten

---

## 📅 Woche 2: GRE-Tunnel & NAT/PAT
### Nataliia
- [ ] GRE Tunnel0 & Tunnel1 (HQ-Seite) konfigurieren
- [ ] Statische Routen für Linz/Graz über Tunnel setzen
- [ ] NAT (Network Address Translation) ACL und Overload konfigurieren
- [ ] Screenshots: `show ip nat translations` (Tabelle der aktiven Adressübersetzungen)

### Anh
- [ ] GRE Tunnel0 (Linz-Seite) konfigurieren
- [ ] Branch-Graz-Router: Basis-Konfiguration & DHCP
- [ ] GRE Tunnel1 (Graz-Seite) konfigurieren
- [ ] Connectivity-Check: PC6 (Graz) zu HQ-Wien

---

## 📅 Woche 3: ACL & Security
### Nataliia
- [ ] ACL (Access Control List) für File-Server erstellen (Externer Block)
- [ ] Security-Dokumentation (Konzeptbeschreibung)
- [ ] Screenshots: `show access-lists`

### Anh
- [ ] Port Security (Sicherheitsfunktion an Switch-Ports) auf allen Switches aktivieren
- [ ] Inter-Site Tests (Ping/HTTP zwischen allen Standorten)
- [ ] Test: Port err-disabled (Status bei Sicherheitsverletzung) provozieren und dokumentieren

---

## 📅 Woche 4: Abschluss
- [ ] **Review:** Alle Testtabellen finalisieren
- [ ] **Cleanup:** Packet Tracer Datei (Beschriftungen aufräumen)
- [ ] **Abgabe:** Gesamtdokumentation zusammenführen