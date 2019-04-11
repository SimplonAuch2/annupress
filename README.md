# Annuaire Wordpress


Il vous est demandé de mettre en oeuvre un site à l'aide du CMS Wordpress.
Sur la page d'accueil doivent s'afficher les contacts disponibles dans
la table wp_annuaire fournie. Pour cela, sont attendus la mise en oeuvre 
des moyens suivants :
- création d'un plugin Wordpress
- utilisation d'un SHORTCODE
- connexion à la base de données via wpdb



## Documentation

Mots-clés pour recherche Google : wordpress codex

- [créer un plugin Wordpress](https://www.wpnormandie.fr/comment-creer-un-simple-plugin-wordpress/)
- [créer un shortcode](https://codex.wordpress.org/Shortcode_API)
- [connexion SQL](https://codex.wordpress.org/Class_Reference/wpdb)



## Script SQL

```
CREATE TABLE `wp_annuaire` (
  `id` int(11) NOT NULL,
  `prenom` varchar(100) NOT NULL,
  `nom` varchar(100) NOT NULL,
  `mail` varchar(100) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1;

INSERT INTO `wp_annuaire` (`id`, `prenom`, `nom`, `mail`) VALUES
(1, 'Marcel', 'Rodriguez', 'contact@rodrigo.com'),
(2, 'Michel', 'Tournier', 'lastar@planetaire.org'),
(3, 'Julie', 'Lila', 'lilali@lololu.net');
```
