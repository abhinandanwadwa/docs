---
title: Zusammenführen mehrerer persönlicher Konten
intro: Wenn du separate Konten für die Arbeit und für die private Nutzung besitzt, kannst du die Konten zusammenführen.
redirect_from:
- /articles/can-i-merge-two-accounts
- /articles/keeping-work-and-personal-repositories-separate
- /articles/merging-multiple-user-accounts
- /github/setting-up-and-managing-your-github-user-account/merging-multiple-user-accounts
- /github/setting-up-and-managing-your-github-user-account/managing-user-account-settings/merging-multiple-user-accounts
- /account-and-profile/setting-up-and-managing-your-github-user-account/managing-user-account-settings/merging-multiple-user-accounts
versions:
  fpt: '*'
  ghec: '*'
topics:
- Accounts
shortTitle: Merge multiple personal accounts
ms.openlocfilehash: 71e2b280fad682f3ee8e9ac85141aedc3bde3d06
ms.sourcegitcommit: dc42bb4a4826b414751ffa9eed38962c3e3fea8e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/13/2022
ms.locfileid: "145165029"
---
{% tip %}

{% ifversion ghec %}

**Tipp:** {% data variables.product.prodname_emus %} ermöglichen es einem Unternehmen, eindeutige persönliche Konten für seine Mitglieder über einen Identitätsanbieter (IdP) bereitzustellen. Weitere Informationen findest du unter [Informationen zu Enterprise Managed Users](/admin/identity-and-access-management/managing-iam-with-enterprise-managed-users/about-enterprise-managed-users). Für andere Anwendungsfälle wird empfohlen, nur ein Benutzerkonto für die Verwaltung persönlicher und beruflicher Repositorys zu verwenden.

{% else %}

**Tipp:** Es wird empfohlen, nur ein Benutzerkonto für die Verwaltung persönlicher und beruflicher Repositorys zu verwenden. 

{% endif %}

{% endtip %}

{% warning %}

**Warnung:** 
- Organisations- und Repositoryzugriffsberechtigungen können nicht zwischen Konten übertragen werden. Wenn das Konto, das Du löschen möchtest, über eine vorhandene Zugriffsberechtigung verfügt, muss ein Organisationsbesitzer oder Repositoryadministrator das Konto einladen, das Du beibehalten möchtest.
- Alle Commits, die mit einer über GitHub bereitgestellten `noreply`-E-Mail-Adresse erstellt wurden, können nicht von einem Konto in ein anderes übertragen werden. Wenn für das Konto, das du löschen möchtest, die Option **"Keep my email address private"** (Meine E-Mail-Adresse privat halten) verwendet wird, ist es nicht möglich, die von dem Konto erstellten Commits an das Konto zu übertragen, das Du behalten möchtest.

{% endwarning %}

1. [Übertrage alle Repositorys](/articles/how-to-transfer-a-repository) aus dem Konto, das Du löschen möchtest, in das Konto, das Du behalten möchtest. Issues, Pull Requests und Wikis werden ebenfalls übertragen. Überprüfe, ob die Repositorys in dem Konto, das Du behalten möchtest, vorhanden sind.
2. [Aktualisiere die Remote-URLs](/github/getting-started-with-github/managing-remote-repositories) in allen lokalen Klonen der Repositorys, die verschoben wurden.
3. [Lösche das Konto](/account-and-profile/setting-up-and-managing-your-personal-account-on-github/managing-personal-account-settings/deleting-your-personal-account), das Du nicht mehr verwenden möchtest.
4. Um dem neuen Konto frühere Commits zuzuweisen, füge die E-Mail-Adresse hinzu, die Du zum Erstellen des Commits für das Konto verwendet hast, das Du beibehältst. Weitere Informationen findest du unter [Warum werden meine Beiträge nicht auf meinem Profil angezeigt?](/account-and-profile/setting-up-and-managing-your-github-profile/managing-contribution-graphs-on-your-profile/why-are-my-contributions-not-showing-up-on-my-profile#your-local-git-commit-email-isnt-connected-to-your-account)

## <a name="further-reading"></a>Weiterführende Themen

- "[Unterschiedliche Arten von {% data variables.product.prodname_dotcom %}-Konten](/articles/types-of-github-accounts)"
