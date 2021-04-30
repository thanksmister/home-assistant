<div align="center">
    <figure>
        <div>
            <img src="/images/icon_ha.png" alt="" width="128" height="128" />
        </div>
    </figure>
</div>
<h2 align="center">
   Procédure d'installations, configurations et matériel<br/>pour Home Assistant<br/><sup>par Mathieu Longpré</sup>
</h2>

## Table des matières

1. **[Introduction](#introduction)**
2. **[Dell Wyse 7020](https://github.com/logicup-connected/home-assistant/blob/main/WYSE-7020.md)**: présentation du matériel


## Introduction
En tant qu'utilisateur de Home Assistant depuis 2019, j'ai vite réalisé que bien que s'agisse d'une simple intégration domiciliaire, le succès de mon installation et de cette aventure résidait tout d'abord dans une bonne documentation. Ce dépôt se veut ainsi un partage des différents chapitres du développement de mon intégration.
En 2020 l'équipe de développement a voulu éclaircir les différents types d'installation de Home Assistant. Avant d'aller plus loin, il est important de comprendre en quoi consiste le différentes installations:<br/><br/>
**Home Assistant:** Il s'agit de l'installation la plus complète qui consiste à dédier une machine physique, ou virtuelle, l'ensemble de la solution sous la forme d'un système d'exploitation<br/>
**Home Assistant Container:** Se limite à l'installation du noyau principal sous forme de conteneur<br/>
**Home Assistant Core:** Se limite à l'installation du noyau principal directement sous Python<br/>
**Home Assistant Supervised:** Consiste à installer l'ensemble de la solution dans un système d'exploitation autre que celui développé à cette fin. À ce jour, seul Debian est supporté, et ainsi fortement recommandé<br/><br/>

