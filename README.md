# Lost and Found

## Authors

* Robert Norte-Peterson
* Henry Qin

## Purpose

Our app aims to help users find their lost items, as well as providing an outlet for users to return lost items to their owner.

## Features

Users will have the ability to post items as either "lost" or "found". Each item will have an associated name, a description, time found/last seen, picture (optional), contact info, and coordinates if found.

Possible comment section for each item.

Users will only be shown items lost or found within a radius of 10 miles from their location.

Incentives.

## Control Flow

Start at the initial screen with our app's name. Default view routes to a table view of all the current lost items. Swiping left will bring the user to a table view of all the found items. Swiping back returns to the lost items.

Tapping an individual item routes the user to a view of the item containing all of the information about the item.

An add button will route the user to a view which creates a new item. Will contain text fields for the name and description, date field for date last seen/found, drop down box for either lost or found, an optional image upload, and a coordinates selection. When saved, routes back to the table view of the items.

A map view button which displays all of the items pinned on a map. When in map view, the map view button will become a table view button if the user wishes to switch back to the table view. (vice versa)

A search bar to search for certain items.

## Implementation

### Model
* Item.swift

### View
* LostItemsTableView
* FoundItemsTableView
* AddNewItemView
* IndividualItemView
* LostItemsMapView

### Controller
* LostItemsViewController
* FoundItemsViewController
* LostFoundSwipeViewController
* AddNewItemViewController
* LostItemsMapViewController

