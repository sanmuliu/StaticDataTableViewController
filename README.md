StaticDataTableViewController
=============================

Enables to hide static cells

This class enables to hide/show static cells (created in IB, using the option Content : Static cells) for UITableView

Usage

just subclass your UITableViewController

@interface MyViewController : StaticDataTableViewController

than you can use methods

<code>@interface StaticDataTableViewController : UITableViewController

- (BOOL) cellIsHidden:(UITableViewCell *)cell;</code>

- (void) cell:(UITableViewCell *)cell setHidden:(BOOL)hidden;

- (void) reloadDataAnimated;

@end


to hide/show specific cells, to which you have an outlet

<code>
[self cell:self.outletToMyStaticCell1 setHidden:hide];
[self cell:self.outletToMyStaticCell2 setHidden:hide];
[self reloadDataAnimated];
</code>
