# Stage Licence 2 Informatique

J'ai réalisé mon stage de 2 mois de licence 2 au sein du CReSTIC à l'URCA.
Mon sujet était : "Développement et déploiement sur robot quadrupède Lite3"

Je devais développer des mouvements sur le Lite3 qui étaient "perdus" depuis la dernière mise à jour. Etant donné que l'application mobile (qui est fermée) ne faisait pas faire les mouvements au Lite3, j'ai présumé que le problème venait du robot lui même.

Vous pouvez voir plus d'informations sur mon [rapport de stage]().

Plusieurs vidéos sont présentes dans le dossier [doc](/doc/).

J'ai fork 3 repos afin de réaliser de la documentation en français afin de faciliter le travail d'une personne souhaitant réaliser un travail du même type et/ou approfondir le travail que j'ai réalisé.
- [rl_training](https://github.com/Rav3nPho3nix/rl_training)
- [Lite3_rl_deploy](https://github.com/Rav3nPho3nix/Lite3_rl_deploy)
- [gamepad](https://github.com/Rav3nPho3nix/gamepad)

# Conclusion

Durant l'avant dernier jour de mon stage, un développeur de chez DeepRobotics m'a envoyé le lien vers une documentation : les valeurs UDP pour la communication entre le retroid gamepad et le Lite3.

Ces [documents](https://alidocs.dingtalk.com/i/p/OlnXRxOLAljEbGLp/docs/YndMj49yWjPnDl2nIM65wX17J3pmz5aA) contiennent donc les codes UDP à donner pour que le Motion Host puisse lancer les mouvements. Le problème venait donc de l'application mobile et non du robot. Etant donné qu'elle est fermée, il est nécessaire de refaire une application mobile de zéro, ouverte, afin que les modifications soient possibles.

Pour récupérer le flux vidéo, il est possible de le récupérer directement via RTSP avec une commande ressemblante :
```bash
vlc rtsp://ROBOT_IP:PORT/live
```

Un prochain sujet de stage sur le Lite3 pourrait donc être le développement d'une application mobile ouverte.

Je suis quelque peu décu d'avoir trouvé cela à la toute fin de mon stage, rendant une partie de mon stage "inutile" car les mouvements que j'ai recrées sont toujours fonctionnels. J'ai cependant apprécié tout ce processus de recherche et de remise en question.