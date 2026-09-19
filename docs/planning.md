# Planning prévisionnel — La Socketterie

```mermaid
gantt
    title Planning prévisionnel du projet La Socketterie
    dateFormat  YYYY-MM-DD
    axisFormat  %d/%m
    excludes    weekends

    section Cadrage
    Analyse du besoin                              :done, t01, 2026-09-21, 2d
    Architecture technique                        :done, t02, after t01, 2d
    Mise en place dépôt et environnements          :done, t03, after t02, 2d

    section UX / UI
    Parcours UX                                    :crit, t04, 2026-09-21, 3d
    Wireframes                                     :active, t05, after t04, 3d
    Maquettes UI                                   :t06, after t05, 6d

    section Socle e-commerce
    Installation et configuration PrestaShop       :active, t07, 2026-09-25, 3d
    Catalogue et catégories                        :t10, after t07, 4d
    Gestion des comptes clients                    :t11, after t10, 3d
    Panier et tunnel de commande                   :t12, after t11, 4d
    Intégration Stripe                             :t13, after t12, 3d
    Gestion des commandes                          :t14, after t13, 3d
    Factures                                       :t15, after t14, 2d
    Export comptabilité CSV                        :t16, after t15, 2d

    section Front-office
    Intégration du thème                           :t08, after t06, 8d
    Responsive                                     :t09, after t08, 4d
    Pages CMS                                      :t18, after t08, 3d
    Formulaire de contact                          :t19, after t18, 1d

    section Administration
    Gestion des rôles internes                     :t17, after t11, 2d

    section Qualité
    SEO technique                                  :t20, after t09, 2d
    Optimisation performances et écoconception     :t21, after t20, 3d
    Sécurité                                       :t22, after t17, 2d
    Tests fonctionnels                             :t23, after t16, 5d
    Corrections                                    :t24, after t23, 5d

    section Livraison
    Recette client                                 :crit, t25, after t24, 2d
    Mise en production                             :crit, t26, after t25, 2d
    Documentation                                  :t27, after t26, 1d

    section Jalons
    Version présentable pour le tournage TV       :milestone, m1, 2026-12-21, 0d
    Date limite mise en production                :milestone, m2, 2027-01-21, 0d
