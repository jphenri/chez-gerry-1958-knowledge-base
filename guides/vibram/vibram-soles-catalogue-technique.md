# Génération d'une version "Catalogue technique" du dataset Vibram en Markdown

content_catalogue = f"""# Catalogue Technique des Semelles Vibram
**Version:** {today}  
**Source:** chezgerry1958.com  
**Auteur:** Philipe Moreau Latreille / Chez Gerry 1958  
**Objectif:** Référence interne pour la présentation des semelles Vibram disponibles en atelier.  

---

## 🧱 Catégories principales
| Catégorie | Description |
|------------|--------------|
| **Lug** | Semelles à crampons profonds offrant une traction maximale pour le travail, l’extérieur et les conditions hivernales. |
| **Wedge** | Semelles compensées sans talon séparé, légères et confortables, idéales pour un usage quotidien. |
| **Hybrid** | Combinaison de motifs plats et crantés pour un équilibre entre confort urbain et adhérence. |
| **Flat** | Semelles lisses ou légèrement texturées, typiques des chaussures habillées ou casual. |
| **Heel** | Talons ou demi-semelles de remplacement, souvent utilisés sur les modèles classiques ou heritage. |
| **Performance** | Semelles techniques modernes conçues pour la randonnée, le sport ou les environnements extrêmes. |

---

## 🥾 Tableau des semelles Vibram

| Code | Nom | Catégorie | Meilleur usage | Épaisseur (mm) | Notes techniques |
|------|-----|------------|----------------|----------------|------------------|
| 100 | Montagna Full Lug | Lug | Work, Outdoor, Winter | 8.0 | Semelle Vibram iconique, crampons profonds, résistance extrême à l’usure. |
| 1136 | Montagna Block | Lug | Outdoor, Heritage, Winter | 6.5 | Variante plus souple du modèle 100, bonne traction sur neige et sol humide. |
| 430 | Mini Lug | Hybrid | City, Winter | 5.5 | Profil discret, parfait pour bottes urbaines et chaussures de ville robustes. |
| 700 | Cork Nitrile | Flat | City, Heritage, Casual | 4.0 | Semelle Red Wing classique, excellente adhérence sur sol sec. |
| 705 | Nitrile Cork Half Sole | Flat | Dress, Casual | 3.5 | Demi-semelle durable pour ressemelage de chaussures habillées. |
| 4014 | Christy Wedge | Wedge | Comfort, Casual, Heritage | 6.0 | Semelle emblématique des Red Wing Moc Toe, très légère et amortissante. |
| 2021 | Ripple Sole | Wedge | Style, Cushion, City | 5.0 | Design ondulé, bon amorti et look vintage populaire. |
| 132 | Unit Lug | Lug | Work, Outdoor | 7.0 | Semelle robuste, traction supérieure sur terrain accidenté. |
| 430C | Mini Lug (Compound) | Hybrid | City, Durability | 5.0 | Caoutchouc haute densité pour une usure lente et une meilleure durabilité. |
| 100L | Logger Lug | Lug | Logging, Heavy-duty, Work | 8.5 | Crampons profonds pour terrain forestier, résistance à l’huile et à la chaleur. |
| 700R | Roccia Block | Lug | Mountain, Work, Outdoor | 6.5 | Spéciale randonnée ou bottes d’alpinisme, excellente accroche sur roches. |
| 128 | Morbido Half Sole | Flat | Dress, Lightweight | 3.0 | Souple, discrète, adaptée aux souliers légers. |
| 4013 | Christy Heavy Wedge | Wedge | Comfort, Work, Cushion | 7.0 | Variante renforcée de la Christy, plus durable. |
| 1139 | Fire & Ice | Lug | Extreme Cold, Oil Resistance, Safety | 7.5 | Formulation résistante aux températures extrêmes, idéale pour bottes de sécurité. |
| 1276 | Sierra | Lug | Outdoor, Traction | 6.0 | Profil agressif, polyvalente pour rando et bottes utilitaires. |
| 1245 | Kletterlift | Lug | Mountain, Grip, Outdoor | 6.5 | Classique pour bottes d’alpinisme, très bon grip en descente. |
| 168 | Gumlite Wedge | Wedge | Comfort, Lightweight | 5.5 | Matériau microcellulaire, très léger et souple. |
| 286 | Quabaug Heel | Heel | Durability, Heritage | 4.0 | Talon en caoutchouc dur, durable et stable. |
| 7055 | Sphike RGS | Performance | Trail, Grip, Sport | 4.5 | Technologie Rolling Gait System pour foulée naturelle. |
| 1210 | Arctic Grip | Lug | Ice, Snow, Winter | 7.0 | Caoutchouc exclusif antidérapant sur glace. |
| 186C | Carrarmato | Lug | Mountain, Hiking, Heavy-duty | 7.5 | Design emblématique de Vibram, utilisé sur les bottes d’expédition. |
| 360 | Eton | Flat | Dress, City | 3.0 | Semelle fine pour chaussures de ville élégantes. |
| 289 | Stowe | Hybrid | City, All-season | 5.0 | Bon compromis entre adhérence et souplesse. |
| 430V | Mini Lug Vibram Pro | Hybrid | City, Work | 5.5 | Version professionnelle du Mini Lug, résistance accrue. |
| 148 | Sponge Cushion | Wedge | Comfort, Lightweight | 4.5 | Très bon amorti, utilisée sur chaussures orthopédiques et casual. |

---

### 🧩 Notes d’utilisation
- Les épaisseurs peuvent varier légèrement selon le moulage ou la taille de la semelle.  
- Les semelles Vibram sont disponibles en plusieurs composés : **Vi-Lite**, **MorFlex**, **Gumlite**, **Fire & Ice**, etc.  
- Pour chaque ressemelage, vérifier la compatibilité avec le **montage Goodyear**, **Norvégien**, ou **Stitchdown**.  
- Conseiller le client selon l’usage principal : **ville, chantier, plein air, ou style heritage**.

---

**© Chez Gerry 1958 – Cordonnerie haut de gamme | Gatineau, QC**
"""

file_path_catalogue = "/mnt/data/vibram-soles-catalogue-technique.md"
with open(file_path_catalogue, "w", encoding="utf-8") as f:
    f.write(content_catalogue)

file_path_catalogue
