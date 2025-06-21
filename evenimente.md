# 🎃 Ghid Complet Evenimente Server

Acest ghid conține informații detaliate despre toate evenimentele disponibile pe server.

---

## 🌾 EVENIMENT HARVEST FESTIVAL (Chuseok)

### 📋 **Prezentare Generală**

Evenimentul Harvest Festival este un **eveniment festiv** inspirat din tradiția coreeană Chuseok (Festivalul Recoltei). Jucătorii pot participa la misiuni PvE pentru a colecta **Rice Cakes** și să le schimbe pe recompense valoroase.

### 🎯 **Obiectiv Principal**
- **Completează 10 runde** de misiuni consecutive
- **Fiecare rundă** = 2 faze de ucidere monstre
- **Colectează Rice Cakes** pentru recompense speciale

---

## ⚙️ **Sistem de Activare**

### 👤 **Activare GM**
- **Nivel GM**: 5 (Administrator)
- **Comandă**: "Harvest Event Commands" la NPC 20086
- **Status**: Start Event / Stop Event

### 🏃‍♂️ **Pentru Jucători**
- **Eveniment activ**: Flag `harvest_festival` = 1
- **Target automat**: Spre NPC 20086 când evenimentul pornește
- **Reset progres**: Când evenimentul se oprește

---

## 🎮 **Structura Quest-ului**

### 📊 **Progresie Generală**
| Rundă | Faza 1 | Faza 2 | Rice Cakes | Status |
|-------|--------|--------|------------|--------|
| 1-10 | 30 kills (solo) | 60 kills (party) | 2-10 per rundă | Activ |
| 10+ | - | - | - | Complet |

### 🎯 **Faza 1: Solo Kill (30 monstre)**
| Nivel Jucător | Monstru ID | Nume Monstru |
|---------------|------------|--------------|
| 1-10 | 105 | Monstru Începător |
| 11-20 | 301 | Monstru Novice |
| 21-40 | 501 | Monstru Mediu |
| 41-60 | 701 | Monstru Avansat |
| 61-80 | 2202 | Monstru Expert |
| 81+ | 2502 | Monstru Elite |

### 👥 **Faza 2: Party Kill (60 monstre)**
| Nivel Jucător | Monstru ID | Nume Monstru | Cerință |
|---------------|------------|--------------|---------|
| 1-9 | 108 | Boss Începător | Party obligatoriu |
| 10-19 | 109 | Boss Novice | Party obligatoriu |
| 20-30 | 113 | Boss Junior | Party obligatoriu |
| 31-40 | 502 | Boss Mediu | Party obligatoriu |
| 41-50 | 703 | Boss Avansat | Party obligatoriu |
| 51-60 | 707 | Boss Superior | Party obligatoriu |
| 61-70 | 1305 | Boss Expert | Party obligatoriu |
| 71-80 | 2205 | Boss Elite | Party obligatoriu |
| 81-90 | 2501 | Boss Master | Party obligatoriu |
| 91+ | 2503 | Boss Legendary | Party obligatoriu |

---

## 🎁 **Sistemul de Recompense**

### 🍰 **Rice Cakes - Faza 1 (Type 1)**
| Nivel Jucător | Rice Cakes |
|---------------|------------|
| 90+ | 4-7 bucăți |
| 70-89 | 3-6 bucăți |
| 50-69 | 2-4 bucăți |
| 30-49 | 1-3 bucăți |
| 10-29 | 1-2 bucăți |
| 1-9 | 1-2 bucăți |

### 🍰 **Rice Cakes - Faza 2 (Type 2) - Bonus**
| Nivel Jucător | Rice Cakes |
|---------------|------------|
| 90+ | 7-10 bucăți |
| 70-89 | 6-8 bucăți |
| 50-69 | 4-6 bucăți |
| 30-49 | 2-5 bucăți |
| 10-29 | 2-4 bucăți |
| 1-9 | 2-3 bucăți |

---

## 🛒 **Magazin Recompense (NPC 20087)**

### 🎁 **Setul Principal**
| Item ID | Cost Rice Cakes | Descriere |
|---------|-----------------|-----------|
| 50109 | 55 | Set Premium 1 |
| 50110 | 50 | Set Premium 2 |
| 72728 | 45 | Set Mediu 1 |
| 50111 | 30 | Set Basic |

### 🎁 **Setul Extins**
| Item ID | Cost Rice Cakes | Descriere |
|---------|-----------------|-----------|
| 50112 | 65 | Set Elite 1 |
| 50113 | 75 | Set Elite 2 |
| 72724 | 60 | Set Elite 3 |
| 50114 | 75 | Set Elite 4 |
| 50115 | 80 | Set Ultimate |

---

## 🔧 **NPC-uri și Funcții**

### 🎪 **NPC 20086 - Organizator Eveniment**
- **Funcție**: Manager principal eveniment
- **Comenzi GM**: Start/Stop eveniment
- **Quest giver**: Începe rundele de misiuni
- **Progres**: Verifică statusul și primește recompense

### 🛍️ **NPC 20087 - Comerciant Recompense**
- **Funcție**: Schimbă Rice Cakes pe iteme
- **Meniu**: 9 tipuri de recompense disponibile
- **Verificare**: Cantitate Rice Cakes necesare
- **Confirmare**: Schimb sigur cu preview

---

## 📈 **Strategii Recomandate**

### 🟢 **Pentru Începători (Nivel 1-30)**
1. **Faza 1**: Monstre slabi, kill rapid
2. **Faza 2**: Găsește party pentru boss-uri
3. **Recompense**: 3-7 Rice Cakes per rundă
4. **Target**: Set Basic (30 Rice Cakes)

### 🟡 **Pentru Jucători Medii (Nivel 31-70)**
1. **Faza 1**: Monstre medii, experience decent
2. **Faza 2**: Boss-uri cu party stabil
3. **Recompense**: 6-14 Rice Cakes per rundă
4. **Target**: Set Premium (45-55 Rice Cakes)

### 🔴 **Pentru Veterani (Nivel 71+)**
1. **Faza 1**: Monstre puternici, XP excelent
2. **Faza 2**: Boss-uri legendari cu party elite
3. **Recompense**: 10-17 Rice Cakes per rundă
4. **Target**: Set Ultimate (75-80 Rice Cakes)

---

## ⚠️ **Restricții și Cerințe**

### 📋 **Cerințe Generale**
- ✅ **Eveniment activ** (flag-ul trebuie să fie 1)
- ✅ **Nivel minim** 1 (toate nivelele acceptate)
- ✅ **Progres secvențial** (nu poți sări rundele)

### 🚫 **Restricții Faza 2**
- ❌ **Nu merge solo** - Party OBLIGATORIU
- ❌ **Boss-uri puternici** - Cooperare necesară
- ❌ **Kill stealing** - Doar party member primește credit

### 🔄 **Reset Conditions**
- **La logout**: Progres salvat
- **Eveniment oprit**: Reset complet la toate flag-urile
- **Rundă completă**: Reset kill counters pentru următoarea rundă

---

## 📊 **Statistici și Tracking**

### 📈 **Progres Individual**
- **harvest_festival_count**: Rundele completate (0-10)
- **rice_count**: Rice Cakes totale acumulate
- **mob_kill1_count**: Progres Faza 1 (0-30)
- **mob_kill2_count**: Progres Faza 2 (0-60)

### 🎯 **Quest Flags**
- **harvest_festival_mob_complete**: Rundă finalizată (0/1)
- **mob1_info**: Tipul monstrului Faza 1 (1-6)
- **mob2_info**: Tipul monstrului Faza 2 (1-10)

---

## 🏆 **Beneficii Eveniment**

### ✨ **Pentru Jucători**
- **XP farming** organizat și rewarding
- **Party gameplay** încurajat
- **Recompense exclusive** doar din eveniment
- **Progresie clară** cu target-uri concrete

### 🎮 **Pentru Server**
- **Activitate crescută** în perioada evenimentului
- **Cooperare între jucători** prin party requirements
- **Engagement** pe termen lung (10 runde)
- **Balance** - nu e prea ușor, nu e prea greu

---

## 💡 **Tips și Tricks**

### 🎯 **Eficiență Maximă**
1. **Formează party permanent** pentru ambele faze
2. **Coordonează cu guild-ul** pentru organizare
3. **Calculează Rice Cakes** înainte să cheltui
4. **Prioritizează recompensele** după nevoile tale

### 🔥 **Optimizare Timp**
- **Faza 1**: Mergi la zone cu mob density mare
- **Faza 2**: Pregătește party-ul din timp
- **Reset rapid**: Vorbește cu NPC imediat după completare
- **Planificare**: 10 runde = investiție de timp considerabilă

---

*🎃 Evenimentul Harvest Festival oferă o experiență completă de MMO cu PvE grinding, party cooperation și reward system bine balansat!* ✨
