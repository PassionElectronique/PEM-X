# Projet PEM-X : Processeur Éducatif Modulaire eXpérimental

> Projet en cours de développement !!

Le projet "PEM-X" est un :

- **microprocesseur 8 bits**
- avec **uniquement des puces 74HCxx + RAM + ROM**
- qui se veut **100% open-source**, **éducatif**, et **modulaire**

Conçu pour **apprendre l'électronique**, étape par étape.

## 🎯 Architecture en bref

- **Type** : Processeur 8 bits, architecture Harvard modifiée
- **Registres** : 16 registres de 8 bits
- **Mémoires** :
  - 64K×16 bits de ROM (programme)
  - 64K×8 bits de RAM
- **Instructions** : ~30 environ (MOV, ADD, XOR, JMP, CALL, IN/OUT, etc) - CISC compact
- **Drapeaux** : Zéro, Carry, Négatif, Overflow
- **Microcode** : 32 bits, avec 1 à 16 µ-instruction par instruction
- **Périphériques** : 32 slots mappés (RAM + 31 libres), disposant de :
  - bus d'adresse 16 bits
  - bus de données 8 bits

## 🛠️ Avancement projet

### Réalisé :

0. ✅ **Préparation projet** : schéma global, avec recherches préalables

### À faire :

1. ⏳ **Carte support** : Alimentation +5V, distribution des bus d’adresse/données/commande partagés
2. ⏳ **Carte PC + ROM + IR** : Compteur de programme (CP), ROM programme (ROM), registres d’instruction (IR)
3. ⏳ **Carte UC** : Unité de commande (UC), avec Micro-ROM et logique de séquençage intégrés
4. ⏳ **Carte RF** : Register Files (RF), avec 16 registres de 8 bits intégrés
5. ⏳ **Carte ALU** : Unité arithmétique et logique (ALU), avec sortie drapeaux Z, C, N, V (flags zero/carry/neg/ovf)
6. ⏳ **Carte IODS + SP + BTW** : I/O Device Selector (DS), Stack pointer (SP), et ByteToWord (BTW)
7. ⏳ **Carte CLK** : Clock (CLK), fournissant une horloge à 4 MHz
8. ⏳ **Carte RAM** : 8 Ko de RAM (partagée par programme et pile) ; pour rappel, ce sera le périphérique #0, obligatoire pour un bon fonctionnement du processeur (avec utilisation de la pile et autre)
9. ⏳ **Carte Périphérique #1** : Une interface homme-machine, avec des interrupteurs (microswitchs) et/ou bouton poussoirs, ainsi que des voyants et/ou afficheurs 7 segments

> Chaque carte aura son **article dédié** sur [Passion Électronique](https://passionelectronique.fr) avec schémas, photos, et tests réalisés dessus

## 📖 Licence

Licence BY-NC-ND 4.0 CC<br />
Lien : https://creativecommons.org/licenses/by-nc-nd/4.0/deed.fr

## 📬 Contact

- **Site** : [passionelectronique.fr](https://passionelectronique.fr)
- **GitHub** : [PassionElectronique](https://github.com/PassionElectronique)
- **X** : [Jérôme TOMSKI](https://x.com/jerometomski)

---

@2025<br>
Créé par Jérôme TOMSKI
