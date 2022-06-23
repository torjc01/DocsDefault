[![img](https://img.shields.io/badge/Lifecycle-Experimental-339999)](https://www.quebec.ca/gouv/politiques-orientations/vitrine-numeriqc/accompagnement-des-organismes-publics/demarche-conception-services-numeriques)
[![License](https://img.shields.io/badge/Licence-LiLiQ--R-blue)](LICENSE_FR)

---

<div>
    <img src="./images/mcn.png">
</div>

# Sécurité 


It’s becoming increasingly common to add a SECURITY.md file that highlights security-related information for your project. Not only does it give users of your open source project the important security information they need, but it also forces the maintainers to think about how they should deal with security disclosures, updates and general security practices.

Il est de plus en plus courant d'ajouter un fichier `SECURITY.md` qui met en évidence les informations relatives à la sécurité de votre projet. Non seulement cela donne aux utilisateurs de votre projet open source les informations de sécurité importantes dont ils ont besoin, mais cela oblige également les responsables à réfléchir à la manière dont ils doivent gérer les divulgations de sécurité, les mises à jour et les pratiques générales de sécurité.

Améliorez les rapports et corrigez les vulnérabilités lorsqu'elles sont découvertes. Le fichier `SECURITY.MD` doit se trouver dans le répertoire racine de tous les projets open source. Il fournit des directives sur la façon de contacter les projets concernant des problèmes de sécurité ou des bogues.

L'objectif est d'améliorer la sécurité open source en rendant les politiques plus accessibles et en signalant les vulnérabilités de sécurité plus facilement pour tout le monde.

Un fichier `SECURITY.md` doit contenir :

* **Disclosure policy: You need to define the procedure for the person that found security issues, and who the contact is for them. You can configure the ‘security@’ email.**  
    This illustrates the importance of defining the procedure of how an issue reporter can fully disclose security issues responsibly. This should include who to contact and how. This is extremely important as it allows you to gain important feedback from the users of your project.If there’s no easy well-defined way of doing something, it’s easy for us to not bother doing it at all. Others may log the existence of a vulnerability as an open issue, inadvertently making the world aware of it before a fix is available. Make sure you give your project users all the direction they need to give the right information to project maintainers when issues are found.
* **Politique de divulgation : vous devez définir la procédure pour la personne qui a trouvé des problèmes de sécurité, et qui est le contact pour elle. Vous pouvez configurer l'e-mail "security@".**  
    Cela illustre l'importance de définir la procédure permettant à un signaleur de problème de divulguer pleinement les problèmes de sécurité de manière responsable. Cela devrait inclure qui contacter et comment. Ceci est extrêmement important car cela vous permet d'obtenir des retours importants des utilisateurs de votre projet. D'autres peuvent enregistrer l'existence d'une vulnérabilité comme un `open issue`, en informant par inadvertance le monde avant qu'un correctif ne soit disponible. Assurez-vous de donner aux utilisateurs de votre projet toutes les instructions dont ils ont besoin pour donner les bonnes informations aux responsables du projet lorsque des problèmes sont détectés.

* **Security Update policy: You need to define how you intend to update users about new security vulnerabilities as they are found.**   
    Software vulnerabilities are discovered every single day. When a vulnerability is found in your application or library, you have a responsibility to tell the users of your project. They could be using your open source code in production on critical systems. You need to have a well-defined process to share the relevant information to them, including the severity of the vulnerability, the risk it brings, and how to move to a fixed version of your code. Define this process upfront so that the information is pushed to your project users, allowing them to be updated as early as possible about new security vulnerabilities as they are found and fixed. This might be as simple as a security mailing list. A SECURITY.md file is a good home for such info on the repo, and if you have a website, consider an independent page for it – see Express.js’s security page as an example.
* **Politique de mise à jour de sécurité : vous devez définir comment vous souhaitez informer les utilisateurs des nouvelles vulnérabilités de sécurité au fur et à mesure qu'elles sont détectées.**  
    Des vulnérabilités logicielles sont découvertes chaque jour. Lorsqu'une vulnérabilité est détectée dans votre application ou votre bibliothèque, vous avez la responsabilité d'en informer les utilisateurs de votre projet. Ils pourraient utiliser votre code open source en production sur des systèmes critiques. Vous devez disposer d'un processus bien défini pour leur partager les informations pertinentes, y compris la gravité de la vulnérabilité, le risque qu'elle comporte et comment passer à une version fixe de votre code. Définissez ce processus à l'avance afin que les informations soient envoyées aux utilisateurs de votre projet, leur permettant d'être informés le plus tôt possible des nouvelles vulnérabilités de sécurité au fur et à mesure qu'elles sont trouvées et corrigées. Cela peut être aussi simple qu'une liste de diffusion de sécurité. Un fichier SECURITY.md est une bonne maison pour de telles informations sur le dépôt, et si vous avez un site Web, envisagez une page indépendante pour celui-ci.
* **Security-related configuration: This includes settings that users should consider that would impact the security posture of deploying this project.**  
    Security related configurationThe security considerations of your project go beyond your code alone. Users of your open source project likely need to add configuration to your project and create settings in order for it to work as necessary in their environment. You should provide your project users with suggested settings that harden their security posture when deploying this project. Examples include turning on HTTPS, adding an authorization layer and of course replacing default passwords (guidance many MongoDB users wish they’ve gotten). Remember that many users typically have a fairly low understanding of security, so any advice you can pass on will help them greatly.
* **Configuration liée à la sécurité : cela inclut les paramètres que les utilisateurs doivent prendre en compte et qui auraient un impact sur la posture de sécurité du déploiement de ce projet.**  
    Les considérations de sécurité de votre projet vont au-delà de votre code seul. Les utilisateurs de votre projet open source doivent probablement ajouter une configuration à votre projet et créer des paramètres pour qu'il fonctionne selon les besoins dans leur environnement. Vous devez fournir aux utilisateurs de votre projet des paramètres suggérés qui renforcent leur posture de sécurité lors du déploiement de ce projet. Les exemples incluent l'activation de HTTPS, l'ajout d'une couche d'autorisation et bien sûr le remplacement des mots de passe par défaut. N'oubliez pas que de nombreux utilisateurs ont généralement une compréhension assez faible de la sécurité, donc tout conseil que vous pouvez leur transmettre les aidera grandement.
* **Known security gaps & future enhancements. This includes security improvements you haven’t implemented yet.**  
    There’s a tradeoff between giving your users the information they need to secure their environment versus enabling an attacker with suggested attack routes. Always consider how the information you share could be used by both parties.Very rarely are projects in such a state that all the security improvements you want to make have been implemented. It’s important to inform your project users of the security controls that aren’t currently in place. Your users deserve to know the full story so they can make informed decisions about how they use your project. Who knows—you may even get contributions of a security control implementation from your users on the list!
* **Lacunes de sécurité connues et améliorations futures. Cela inclut les améliorations de sécurité que vous n'avez pas encore mises en œuvre.**  
    Il existe un compromis entre donner à vos utilisateurs les informations dont ils ont besoin pour sécuriser leur environnement et activer un attaquant avec des itinéraires d'attaque suggérés. Considérez toujours comment les informations que vous partagez pourraient être utilisées par les deux parties. Il est très rare que des projets soient dans un état tel que toutes les améliorations de sécurité que vous souhaitez apporter aient été mises en œuvre. Il est important d'informer les utilisateurs de votre projet des contrôles de sécurité qui ne sont pas actuellement en place. Vos utilisateurs méritent de connaître toute l'histoire afin qu'ils puissent prendre des décisions éclairées sur la façon dont ils utilisent votre projet. Qui sait, vous pourriez même obtenir des contributions d'une implémentation de sécurité de vos utilisateurs sur la liste !



## Références 



[Add a SECURITY.md file to your Azure Repos https://snyk.io/blog/add-a-security-md-file-to-your-azure-repos/](https://snyk.io/blog/add-a-security-md-file-to-your-azure-repos/)

[Example SECURITY.md (https://github.com/atomist/samples/blob/master/SECURITY.md)](https://github.com/atomist/samples/blob/master/SECURITY.md)

https://github.com/Trewaters/security-README
