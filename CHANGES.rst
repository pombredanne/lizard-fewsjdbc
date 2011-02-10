Changelog of lizard-fewsjdbc
============================


1.3 (unreleased)
----------------

- Showing parameter name in csv/html column header.

- Making explicit that the extracted datetime is GMT+1.

- Added 'period' parameter: the start/end dates are set to -period
  days till now.


1.2 (2011-02-08)
----------------

- Added height/width support to png api call.


1.1 (2011-02-08)
----------------

- Adding better error handling to jdbc queries: they raise errors
  right away now instead of returning -1 or -2 and checking later on
  in the code.

- Supporting date range setting.

- Added csv/html/png output.

- Added implementation of lizard-map's REST api for jdbc sources,
  filters, parameters and locations.

- Added ``.get_locations()`` method to jdbc source model (with the
  rest of the related get_something methods) instead of keeping it in
  the adapter.


1.0.1 (2011-02-02)
------------------

- Added crumbs_prepend (see lizard_ui).


1.0 (2011-01-13)
----------------

- Fixed some points not showing. Working around Mapnik bug #402. Needs
  lizard-map 1.39 or higher.

- Implemented adapter.extent.


0.9.2 (2010-12-09)
------------------

- Fixed not showing all parameters.


0.9.1 (2010-12-08)
------------------

- Bugfix moving operations.


0.9 (2010-12-08)
----------------

- Moved list operations to lizard_map (1.27).

- Added filter_tree_root. The filter_tree_root takes a filter_id as a
  root and loads the tree from that point. Use only if not using
  usecustomfilter.


0.8 (2010-11-10)
----------------

- Bugfix accordion.

- Add tests, make tests independent of external data source.


0.7 (2010-10-18)
----------------

- Bugfix using iso8601.


0.6 (2010-10-18)
----------------

- Change datetime conversion from timetuple to iso8601 parsing
  (timetuple does not always exist).


0.5 (2010-10-15)
----------------

- Use lizard-ui 1.21.


0.4 (2010-10-15)
----------------

- Added option ignore_cache in fews_jdbc page.


0.3 (2010-10-15)
----------------

- Added usecustomfilter option.

- Update fixtures.


0.2 (2010-10-15)
----------------

- Pinned lizard-map and lizard-ui.


0.1 (2010-10-15)
----------------

- Initial library skeleton created by nensskel.  [Jack]

- Added model for Jdbc source.

- Frontpage shows list of Jdbc sources.

- Added tests.

- Each Jdbc source has an own page, where workspace items can be used.

- Basic adapter for Jdbc source implemented: layer, image, values, ...