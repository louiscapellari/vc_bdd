# vc_bdd

## Présentation générale de la base de données
La base de données SIG développée s’inscrit dans une démarche de connaissance, de gestion et de valorisation du territoire. Conçue autour des thématiques environnementales et touristiques, elle a pour vocation de centraliser et d’organiser des données géographiques issues de sources variées afin de produire une information géographique pertinente permettant de mettre en valeur les richesses naturelles, les contraintes environnementales, les espaces protégés ainsi que les équipements liés au tourisme.

## Sources des données utilisées 
- IGN (Institut national de l’information géographique et forestière)
- DDT Savoie (Direction Départementale des Territoires)
- OSM (OpenStreetMap)
- BRGM (Bureau de Recherches Géologiques et Minières)
- INPN (Inventaire National du Patrimoine Naturel)
- CEN (Conservatoire d’Espaces Naturels)

## Détail  de la structure de la base de données et des couches utilisées 
| Schéma | Couche | Contenu / utilité |
|--------|---------|-------------------|
| administratif | cc_hmv (IGN) | Limites intercommunales. |
| administratif | val_cenis (IGN) | Limites communales de Val-Cenis. |
| administratif | zone_habitation (IGN) | Zones urbanisées. |
| administratif | lieux_dits (OSM) | Localisation des lieux-dits, repères toponymiques. |
| administratif | toponymie (OSM) | Référentiel de noms de lieux |
| adresse | ban (IGN) | Base Adresse Nationale, adresses normalisées. |
| adresse | lien_adresse_bati (IGN) | Relation entre adresse et bâtiment. |
| adresse | lien_adresse_parcelle (IGN) | Relation entre adresse et parcelle cadastrale. |
| adresse | lien_adresse_support (IGN) | Liens entre adresses et supports . |
| adresse | lien_bati_parcelle (IGN) | Relation entre bâtiment et parcelle. |
| adresse | voie_nommee (IGN) |  |
| agriculture | cours_eau_bcae (IGN) | Réseau hydrographique lié à la réglementation agricole. |
| agriculture | rpg (IGN) | Registre parcellaire graphique, occupation agricole des sols. |
| alti | lignes_courbes (IGN) | Courbes de niveau. |
| alti | mns (IGN) | Modèle numérique de surface. |
| alti | mnt (IGN) | Modèle numérique de terrain. |
| batiment_topo | borne_recharge (OSM) | Localisation des bornes de recharge électrique. |
| batiment_topo | station_epuration (DDT) | Stations de traitement des eaux usées. |
| batiment_topo | batiment (IGN) | Référentiel bâti. |
| batiment_topo | construc_lineaire (IGN) | Infrastructures linéaires bâties. |
| batiment_topo | construc_ponctuelle (IGN) | Objets bâtis ponctuels. |
| batiment_topo | construc_surfacique (IGN) | Constructions surfaciques hors bâti principal. |
| batiment_topo | erp (IGN) | Établissements recevant du public. |
| batiment_topo | ligne_orographique (IGN) | Crêtes et lignes de partage des eaux. |
| batiment_topo | piste_aerodrome (IGN) | |
| batiment_topo | reservoir (IGN) | Réservoirs d’eau. |
| batiment_topo | stationnement (OSM) |  |
| energie | ligne_electrique (IGN) |  |
| energie | poste_transfo (IGN) | |
| energie | pylones (IGN) | Localisation des pylônes électriques. |
| energie | lampadaire (OSM) | Points lumineux publics. |
| environnement | exploitation_materiaux (BRGM) | Sites d’extraction de matériaux. |
| environnement | mines (BRGM) | Anciennes et actuelles exploitations minières. |
| environnement | pelouses_seches (CEN) |  |
| environnement | sites_geres (CEN) | Espaces naturels gérés par le CEN. |
| environnement | tourbiere (CEN) | Localisation des tourbières. |
| environnement | aire_protec_biotope (DDT) | Périmètres de protection de biotopes. |
| environnement | carriere (DDT) | Sites de carrières. |
| environnement | pastoral_zone_zinf (DDT) | Zones pastorales d’intérêt environnemental. |
| environnement | res_chasse_faune_zinf (DDT) | Réserves de chasse et faune d’intérêt. |
| environnement | zap_pdrr_biodiv (DDT) | Zones agricoles protégées liées à la biodiversité. |
| environnement | zones_humides (DDT) | Zones humides inventoriées. |
| environnement | formation_vegetale (IGN) | Typologies de formations végétales. |
| environnement | haie (IGN) | |
| environnement | parc_reserve (IGN) | |
| environnement | preserv_praries_paturages_n2000 (IGN) | |
| environnement | restriction_drone (IGN) | |
| environnement | arretes_protec_biotope (INPN) | Sites sous arrêté de protection de biotope. |
| environnement | sic_n2000 (INPN) | Sites d’Intérêt Communautaire Natura 2000. |
| environnement | zps_n2000 (INPN) | Zones de Protection Spéciale Natura 2000. |
| environnement | parcs_nationaux (INPN) | Limites des parcs nationaux. |
| environnement | region_biogeo (INPN) | Régions biogéographiques. |
| environnement | znieff_type1 (INPN) | Zones naturelles d’intérêt écologique (type 1). |
| environnement | znieff_type2 (INPN) | Zones naturelles d’intérêt écologique (type 2). |
| environnement | elems_naturels (OSM) | Éléments naturels. |
| environnement | lieux_naturels (OSM) | Lieux à caractère naturel. |
| environnement | sommets (OSM) | Localisation des sommets. |
| foret | foret_protec (DDT) | Forêts protégées. |
| foret | foret_publique (IGN) | Forêts publiques. |
| foret | foret (OSM) | Polygones de forêts OSM. |
| geologie | bss (BRGM) | Banque de données du sous-sol. |
| geologie | carhab (BRGM) | Cartographie des habitats naturels. |
| geologie | carte_litho_1m (BRGM) | Carte lithologique au 1:1 000 000. |
| geologie | geo050k_harm_073_p_divers (BRGM) |  |
| geologie | geo050k_harm_l_divers (BRGM) | Lignes géologiques diverses. |
| geologie | geo050k_harm_l_fgeol (BRGM) | Faille et structures géologiques. |
| geologie | geo050k_harm_p_struct (BRGM) | |
| geologie | geo050k_harm_s_fgeol | Surfaces géologiques spécifiques. |
| geologie | patrimoine_geologique (INPN) | Sites d’intérêt géologique. |
| geologie | falaises (OSM) | Localisation de falaises. |
| geologie | plages (OSM) | Localisation de plages. |
| hydro | station_epuration (DDT) | Stations d’épuration. |
| hydro | bassin_versant (IGN) | Délimitation des bassins versants. |
| hydro | cours_eau (IGN) | Réseau hydrographique principal. |
| hydro | details_hydro (IGN) | Détails complémentaires hydrographiques. |
| hydro | glacier (IGN) | Localisation des glaciers. |
| hydro | inpe (IGN) | Inventaire national des plans d'eau |
| hydro | noeud_hydro (IGN) | Nœuds hydrographiques. |
| hydro | reservoir (IGN) | Réservoirs d’eau. |
| hydro | station_hydro (IGN) | Stations de mesure hydrologique. |
| hydro | surf_hydro (IGN) | Surfaces en eau. |
| hydro | toponymie_hydro (IGN) | Toponymie des cours d’eau. |
| hydro | troncon_hydro (IGN) | Tronçons de cours d’eau. |
| hydro | chute_eau (OSM) | Localisation de chutes d’eau. |
| hydro | eau_potable (OSM) | Points liés à l’eau potable. |
| imagerie | ortho_irc | Orthophotographies infrarouge. |
| imagerie | ortho_rvb | Orthophotographies couleurs naturelles. |
| imagerie | carto_fonctions_ndvi_regularite | Indice de végétation NDVI. |
| imagerie | prob_presence_seuille_milieux_humides |  |
| mobilite | aerodrome (IGN) | Localisation des aérodromes. |
| mobilite | troncon_route (IGN) | Réseau routier IGN. |
| mobilite | voie_nommee (IGN) | Routes avec noms. |
| mobilite | routes (OSM) | Réseau routier OSM. |
| mobilite_durable | voie_ferree_nommee (IGN) | Réseau ferré. |
| mobilite_durable | arret_bus (OSM) | Localisation des arrêts de bus. |
| mobilite_durable | voie_velo (OSM) | Réseau cyclable. |
| occupation_du_sol | corine_land_cover_2018 | Occupation du sol Corine Land Cover. |
| occupation_du_sol | ocs_ge (IGN) | Occupation du sol à grande échelle. |
| occupation_du_sol | zone_construite (IGN) | Zones bâties. |
| parcellaire | divcad | Données cadastrales (divisions). |
| parcellaire | parcelle | Polygones cadastraux. |
| parcellaire | localisant | |
| patrimoine | ruine_chalet (DDT) | Chalets en ruine. |
| patrimoine | monum_histo (DDT) | Monuments historiques. |
| risques | cavites_localisee (BRGM) | Cavités souterraines. |
| risques | geo050k_harm_l_struct (BRGM) | Structures géologiques. |
| risques | geo050k_harm_s_surch (BRGM) | Surfaces de surcharge. |
| risques | gisements_gites_indices (BRGM) | Gisements et indices miniers. |
| risques | mvmt_terrain (BRGM) | Mouvements de terrain. |
| risques | digue_inond_sub (DDT) | Digues de protection contre les inondations. |
| risques | ppri (DDT) | Plans de prévention du risque inondation. |
| risques | pprn (DDT) | Plans de prévention des risques naturels. |
| tourisme_sport_culture | domaine_skiable (DDT) | Domaines skiables. |
| tourisme_sport_culture | piste_ski (DDT) | Pistes de ski. |
| tourisme_sport_culture | remontee_meca (DDT) | Remontées mécaniques. |
| tourisme_sport_culture | gr_rando | Sentiers de GR. |
| tourisme_sport_culture | detail_orographique (IGN) | Relief détaillé. |
| tourisme_sport_culture | infos_tourisme (IGN) | Points d’information touristique. |
| tourisme_sport_culture | musee (OSM) | Localisation de musées. |
| tourisme_sport_culture | site_archeo (IGN+OSM) | Sites archéologiques. |
| tourisme_sport_culture | refuges_abris (IGN) | Refuges et abris. |
| tourisme_sport_culture | sentiers_ign (IGN) | Réseau de sentiers de randonnée. |
| tourisme_sport_culture | terrain_sport (IGN) | Infrastructures sportives. |
| tourisme_sport_culture | toponym_service_activ (IGN) | Lieux touristiques nommés. |
| tourisme_sport_culture | transport_cable (IGN) | Téléphériques, télécabines, remontées mécaniques. |
| tourisme_sport_culture | za_zi (IGN) | Zones d’activités économiques. |
| tourisme_sport_culture | campings (OSM) | Campings. |
| tourisme_sport_culture | caravane (OSM) | Aires de caravanes. |
| tourisme_sport_culture | connaissance_territoire (OSM) | Points de connaissance du territoire. |
| tourisme_sport_culture | forts_chateaux (OSM) | Forts et châteaux. |
| tourisme_sport_culture | hotel_hostel_guesthouse (OSM) | Hébergements touristiques. |
| tourisme_sport_culture | install_tourisme (OSM) | Installations touristiques diverses. |
| tourisme_sport_culture | oeuvre_art (OSM) | Localisation d'Œuvres d’art. |
| tourisme_sport_culture | pt_vue (OSM) | Points de vue panoramiques. |
| tourisme_sport_culture | refuges (OSM) | Refuges de montagne. |
| tourisme_sport_culture | refuges_partiels (OSM) | Refuges partiels. |
| tourisme_sport_culture | sentiers_osm (OSM) | Sentiers de randonnée OSM. |
| tourisme_sport_culture | trail (OSM) | Parcours de trail. |
| tourisme_sport_culture | sentiers_rando | |
| trame_verte_et_bleu | inv_frayeres (DDT) | Inventaire des frayères. |
| urbanisme | plu_ponctuel (DDT) | Prescriptions ponctuelles PLU. |
| urbanisme | plu_prescr_lineaire (DDT) | Prescriptions linéaires PLU. |
| urbanisme | plu_zonaga_urba (DDT) | Zonage d’urbanisme. |

## Prérequis  
- Disposer de PostgreSQL 17.
- Disposer de PG Admin 4 (dans le cas de ce tutoriel)

## Instructions d'installation
- Depuis PG Admin 4, créer une nouvelle base de données intitulée "sig_vc"
<img width="1106" height="148" alt="12" src="https://github.com/user-attachments/assets/b68bf31b-a094-44f7-a9bd-67bdf3c758d2" />
<img width="1414" height="1108" alt="13" src="https://github.com/user-attachments/assets/f201052d-2b10-4384-a437-1b5bacb7f16f" />
- Depuis la base de données "sig_vc", restaurer la base de données depuis le fichier "sig_vc.backup"
<img width="956" height="454" alt="14" src="https://github.com/user-attachments/assets/f61c91ea-559d-4a57-ae08-d67a4f0b3eca" />
<img width="1544" height="1064" alt="15" src="https://github.com/user-attachments/assets/787364cc-0dfe-43cf-846f-cffad79f99d3" />
- Depuis QGIS, ajoutez la base de données "sig_vc" :
<img width="892" height="1512" alt="16" src="https://github.com/user-attachments/assets/7303ac3f-76ad-49ea-b95a-66b2f549e4ac" />
- Vous devriez maintenant pouvoir disposer des couches présentes dans la base de données
  
## Précautions 
Les couches rasters ne sont pas incluses dans le dump. 
