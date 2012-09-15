Init.

1. Add remote and fetch

    git remote add -f log.core git@git.xgbi.fr:nexgen/modules/org.xgbi.nexgen.support.log.core.git

2. Checkout remote branches in local branches (subtree/..)

    git co -b subtree/log.core.develop log.core/develop

3. Add it with a prefix

    git subtree add --prefix=org.xgbi.nexgen.support.log.core subtree/log.core.develop

4. Do your stuff (modification, ...)

5. Time to split !

    git subtree split --prefix=org.xgbi.nexgen.support.log.core --annotate="[support.i18n]" --rejoin -b subtree/log.core.develop

6. Push modification to subtree repository

    git push log.core subtree/log.core.develop:develop

