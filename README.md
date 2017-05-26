RunQCharts - QCharts Standard
=============================
RunQCharts represents a Symfony (2.7.*) project, in which QCharts
has been implemented. This is only to illustrate the Standard way
of implementing QCharts in a Symfony project.

Powered by QCharts.

--------------------------------------------------

NOTES:
------

RunQCharts includes a ```composer.json``` file and the corresponding
```composer.lock``` file used to get RunQCharts up and running.
- The only installation you should follow would be with composer without
dev dependencies!
```composer install```
- And, of course, set up your parameter's file ```parameters.yml```.
- Dump Assetic, ```app/console assetic:dump```.
- Install Assets, ```app/console assets:install```.
- Set up the database with `app/console doctrine:schema:create` or `app/console doctrine:schema:update`
- This QCharts implementation uses ApiBundle, hence no ApiDoc from
Nelmio is implemented, for more information about the matter, check out
the QCharts Repo.

--------------------------------------------------

QCharts
-------
- Install QCharts with composer in your project ```composer install arnulfosolis/qcharts @dev```.
- Or check out the Qchart's repo: https://github.com/arnulfojr/qcharts
- Or Packagist's: https://packagist.org/packages/arnulfosolis/qcharts

ApiHistogram
------------
RunQCharts is powered by ApiHistogram too, feel free to check it out.
- Install ApiHistogram with composer in your project ```composer install arnulfosolis/apihistogram @dev```.
- Or check out the Qchart's repo: https://github.com/arnulfojr/apihistogram
- Or Packagist's: https://packagist.org/packages/arnulfosolis/apihistogram

---------------------------------------------------

Contact
=======
Arnulfo Solis.
Email: arnulfojr@kuzzy.com
Twitter: @arnulfojr
