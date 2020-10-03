# GIT FLOW

git flow init - inicia um projeto git com gitflow
git flow feature start <nome_feature> - cria uma branch de feature com o nome da feature desejada
git flow feature publish - faz push das features no git
git flow feature finish - finalizo as features e faz merge com develop e deleta branch (local e online)
git flow release start <numero_versao> - cria release
git flow release finish <numero_versao> - finalizo a release e deleta branch (local e online) = abre varias janelas para adicionar nome da release, tag, etc