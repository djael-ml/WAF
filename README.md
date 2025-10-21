# 🛡️ WAF - Web Application Firewall

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![Status](https://img.shields.io/badge/status-in%20development-orange.svg)]()

Un Web Application Firewall (WAF) open source moderne et performant, conçu pour protéger vos applications web contre les menaces courantes.

## ⚠️ Statut du Projet

**Ce projet est actuellement en développement actif.** Les fonctionnalités sont susceptibles de changer et l'API n'est pas encore stable. N'utilisez pas en production pour le moment.

## 📋 Fonctionnalités Prévues

- 🔒 Protection contre les injections SQL
- 🚫 Détection et blocage des attaques XSS
- 🛑 Protection contre les attaques CSRF
- 📊 Système de logging et monitoring
- ⚡ Détection des attaques DDoS
- 🔍 Analyse des patterns de requêtes suspects
- 📝 Règles personnalisables
- 🎯 Liste blanche/noire d'IPs
- 📈 Dashboard de visualisation (à venir)

## 🚀 Installation
```bash
# Cloner le repository
git clone https://github.com/votre-organisation/waf.git
cd waf

# Créer un environnement virtuel
python -m venv venv
source venv/bin/activate  # Sur Windows: venv\Scripts\activate

# Installer les dépendances
pip install -r requirements.txt
```

## 💻 Utilisation
```python
# Exemple d'utilisation basique (à venir)
from waf import WAF

# Initialiser le WAF
firewall = WAF()

# Configurer les règles
firewall.configure(rules="config/rules.yaml")

# Démarrer la protection
firewall.start()
```

## 🛠️ Configuration

La configuration se fait via un fichier YAML :
```yaml
# config/rules.yaml
rules:
  sql_injection:
    enabled: true
    severity: high
  
  xss_protection:
    enabled: true
    severity: high
  
  rate_limiting:
    enabled: true
    max_requests: 100
    window: 60  # secondes
```

## 📚 Documentation

La documentation complète sera disponible prochainement sur notre [wiki](https://github.com/votre-organisation/waf/wiki).

## 🤝 Contribution

Les contributions sont les bienvenues ! N'hésitez pas à :

1. Fork le projet
2. Créer une branche pour votre fonctionnalité (`git checkout -b feature/AmazingFeature`)
3. Commit vos changements (`git commit -m 'Add some AmazingFeature'`)
4. Push vers la branche (`git push origin feature/AmazingFeature`)
5. Ouvrir une Pull Request

### Guidelines de Contribution

- Respecter le style de code Python (PEP 8)
- Ajouter des tests pour les nouvelles fonctionnalités
- Mettre à jour la documentation
- S'assurer que tous les tests passent avant de soumettre

## 🧪 Tests
```bash
# Lancer les tests
pytest

# Avec couverture
pytest --cov=waf tests/
```

## 📝 Roadmap

- [ ] Module de détection d'injection SQL
- [ ] Module de protection XSS
- [ ] Système de règles configurables
- [ ] Interface web de monitoring
- [ ] API REST pour la gestion
- [ ] Support Docker
- [ ] Documentation complète
- [ ] Tests unitaires et d'intégration

## 👥 Auteurs

- [@djael-ml](https://github.com/djael-ml)
- [@MedusaSH](https://github.com/MedusaSH)

## 📄 Licence

Ce projet est sous licence MIT. Voir le fichier [LICENSE](LICENSE) pour plus de détails.

## 🙏 Remerciements

- Merci à tous les contributeurs qui participent à ce projet
- Inspiré par les meilleurs WAF open source existants

## 📞 Contact

Pour toute question ou suggestion, n'hésitez pas à ouvrir une issue sur GitHub.

---

**Note:** Ce projet est en développement actif. Les fonctionnalités et l'API peuvent changer sans préavis.
