To install this module, you need the modules `currency_monthly_rate` and
 to be available in your system.

To configure this module, you need to flag a company as Consolidation in the
Accounting settings.

Then, you should define a consolidation difference account and a consolidation
journal on the consolidation company, and create consolidation profiles for
each subsidiary you want to consolidate.

For each subsidiary to consolidate, make sure the related partner of the
company has no company_id defined.

Afterwards, you should define a consolidation account from your consolidation
company, on every active account of the subsidiaries.

You can then use the 'Consolidation : Checks' wizard in Accounting > Adviser to
ensure every active account of your subsidiaries are set, and company partners
have no company defined.

Make sure you also defined currency rates and monthly currency rates on the
currencies used in your subsidiaries, as P&L accounts are consolidated using
monthly rates and B.S accounts using standard 'spot' rates.

Known issues
============

* When saving the accounting settings, the group multi-company will be removed
  from every user if the group isn't implied by the group employes.
* Consolidation manager has access to all the settings, or he wouldn't be able
  to configure the module.
* Types for accounts mapping should be the same