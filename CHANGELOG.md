# Changelog

## v0.3.0 (26/12/2017)

This release has been very long in coming, and brings a whole host of changes, the most notable being the removal of the user dependency on Typelevel Scala and the new angular units.

Libra has it's first contributors!  Thank you **@DanielaSfregola** and **@ldrygala** for your fantastic work! :tada:

### New units

Hours and days are now present in the `imperial` package. We also support angular units!  Thanks to the work of @ldrygala, degrees, arcminues, arcseconds, gradians, radians and turns are now present in the `nonsi` package.

### New Typeclasses
The following spire / algebra typeclasses have been added to `Quantity`
- `Eq`
- `Order`
- `PartialOrder`
- `Signed`
- `AdditiveSemigroup`
- `AdditiveMonoid`
- `AdditiveGroup`
- `AdditiveCSemigroup`
- `AdditiveCMonoid`
- `AdditiveAbGroup`
- `MetricSpace`
- `CoordinateSpace`
- `VectorSpace`
- `InnerProductSpace`

These are dependent on the typeclasses of the underlying numeric type.

### New operations
Quantities now support Euclidean division with spire's `/~` quotient operator


### Upgrades

The scala versions have been upgraded to `2.11.11` and `2.12.4`

The use of `ValueOf`, and consequently the user dependency on Typelevel Scala.  Users can now use the Lightbend Scala compiler.

### Notable PRs

* [#23](https://github.com/to-ithaca/libra/pull/23) Add more typeclasses
* [#27](https://github.com/to-ithaca/libra/pull/27) Remove Typelevel Scala's `ValueOf`
* [#30](https://github.com/to-ithaca/libra/pull/30) Add time units
* [#35](https://github.com/to-ithaca/libra/pull/35) Add Euclidean division
* [#40](https://github.com/to-ithaca/libra/pull/40) Add andular units: degree, arcminute arcsecond by @DanielaSfregola
* [#44](https://github.com/to-ithaca/libra/pull/44) Rename `Unit` to `UnitOfMeasure`
* [#46](https://github.com/to-ithaca/libra/pull/46) Add angular velocity units: degrees per second, arcminutes per second, arcseconds per second by @ldrygala
* [#49](https://github.com/to-ithaca/libra/pull/49) Add angular units: radian by @ldrygala
* [#51](https://github.com/to-ithaca/libra/pull/51) Add angular units: gradian, turn by @ldrygala
* [#53](https://github.com/to-ithaca/libra/pull/53) Add angular velocity units: radians per second, gradians per second, turns per second


## v0.2.0 (23/04/2017)
* Add units and conversions
* Support scalar multiplication
* Make `Quantity` a value class
* Add fractional exponents to dimensions
* Remove metric exponent from `Quantity`

## v0.1.0 (01/03/2017)
* First release
