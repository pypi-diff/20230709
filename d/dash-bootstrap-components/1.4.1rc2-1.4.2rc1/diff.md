# Comparing `tmp/dash-bootstrap-components-1.4.1rc2.tar.gz` & `tmp/dash-bootstrap-components-1.4.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash-bootstrap-components-1.4.1rc2.tar", last modified: Fri Mar 17 22:53:16 2023, max compression
+gzip compressed data, was "dash-bootstrap-components-1.4.2rc1.tar", last modified: Sun Jul  9 21:46:47 2023, max compression
```

## Comparing `dash-bootstrap-components-1.4.1rc2.tar` & `dash-bootstrap-components-1.4.2rc1.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 22:53:16.866473 dash-bootstrap-components-1.4.1rc2/
--rw-r--r--   0 runner    (1001) docker     (123)    10706 2023-03-17 22:51:55.000000 dash-bootstrap-components-1.4.1rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-17 22:51:55.000000 dash-bootstrap-components-1.4.1rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-17 22:51:55.000000 dash-bootstrap-components-1.4.1rc2/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-03-17 22:53:16.866473 dash-bootstrap-components-1.4.1rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-03-17 22:51:55.000000 dash-bootstrap-components-1.4.1rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 22:53:16.854472 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-03-17 22:51:55.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 22:53:16.866473 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Accordion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/AccordionItem.py
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Badge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Breadcrumb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/ButtonGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Card.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/CardBody.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/CardFooter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/CardGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/CardHeader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/CardImg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/CardImgOverlay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/CardLink.py
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Carousel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Checkbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Checklist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Col.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Collapse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Container.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/DropdownMenu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/DropdownMenuItem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Fade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Form.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/FormFeedback.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/FormFloating.py
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/FormText.py
--rw-r--r--   0 runner    (1001) docker     (123)    14945 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/InputGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/InputGroupText.py
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Label.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/ListGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/ListGroupItem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Modal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/ModalBody.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/ModalFooter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/ModalHeader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/ModalTitle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Nav.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/NavItem.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/NavLink.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Navbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/NavbarBrand.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/NavbarSimple.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/NavbarToggler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Offcanvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Placeholder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7200 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Popover.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/PopoverBody.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/PopoverHeader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/RadioButton.py
--rw-r--r--   0 runner    (1001) docker     (123)     9434 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/RadioItems.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Row.py
--rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Select.py
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Spinner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Table.py
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Tabs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11651 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Textarea.py
--rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Toast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Tooltip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   226816 2023-03-17 22:52:40.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/dash_bootstrap_components.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   361180 2023-03-17 22:52:54.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-03-17 22:51:55.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_table.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-17 22:51:55.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-17 22:51:55.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/icons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-03-17 22:51:55.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/themes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 22:53:16.854472 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-03-17 22:53:16.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-03-17 22:53:16.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 22:53:16.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-17 22:53:16.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-17 22:53:16.000000 dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-03-17 22:51:55.000000 dash-bootstrap-components-1.4.1rc2/landing-page.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-17 22:51:55.000000 dash-bootstrap-components-1.4.1rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-03-17 22:53:16.866473 dash-bootstrap-components-1.4.1rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-03-17 22:51:55.000000 dash-bootstrap-components-1.4.1rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 22:53:16.866473 dash-bootstrap-components-1.4.1rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-03-17 22:51:55.000000 dash-bootstrap-components-1.4.1rc2/tests/test_alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-03-17 22:51:55.000000 dash-bootstrap-components-1.4.1rc2/tests/test_components_as_props.py
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-03-17 22:51:55.000000 dash-bootstrap-components-1.4.1rc2/tests/test_navlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-03-17 22:51:55.000000 dash-bootstrap-components-1.4.1rc2/tests/test_popover.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-03-17 22:51:55.000000 dash-bootstrap-components-1.4.1rc2/tests/test_positional_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-03-17 22:51:55.000000 dash-bootstrap-components-1.4.1rc2/tests/test_tooltip.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-17 22:51:55.000000 dash-bootstrap-components-1.4.1rc2/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:46:47.969700 dash-bootstrap-components-1.4.2rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10706 2023-07-09 21:45:19.000000 dash-bootstrap-components-1.4.2rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-09 21:45:19.000000 dash-bootstrap-components-1.4.2rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-09 21:45:19.000000 dash-bootstrap-components-1.4.2rc1/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-07-09 21:46:47.969700 dash-bootstrap-components-1.4.2rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-07-09 21:45:19.000000 dash-bootstrap-components-1.4.2rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:46:47.949700 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-09 21:45:19.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:46:47.965700 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Accordion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/AccordionItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Badge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Breadcrumb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/ButtonGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/CardBody.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/CardFooter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/CardGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/CardHeader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/CardImg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/CardImgOverlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/CardLink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Carousel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Checklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Col.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Collapse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/DropdownMenu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/DropdownMenuItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Fade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/FormFeedback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/FormFloating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/FormText.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14945 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/InputGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/InputGroupText.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/ListGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/ListGroupItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/ModalBody.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/ModalFooter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/ModalHeader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/ModalTitle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Nav.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/NavItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/NavLink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Navbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/NavbarBrand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/NavbarSimple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/NavbarToggler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Offcanvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7200 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Popover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/PopoverBody.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/PopoverHeader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/RadioButton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9434 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/RadioItems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Spinner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11651 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Textarea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Toast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   226866 2023-07-09 21:46:18.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/dash_bootstrap_components.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   361180 2023-07-09 21:46:23.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-07-09 21:45:19.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-09 21:45:19.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-09 21:45:19.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-09 21:45:19.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/themes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:46:47.953700 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-07-09 21:46:47.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-07-09 21:46:47.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 21:46:47.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-09 21:46:47.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-09 21:46:47.000000 dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-07-09 21:45:19.000000 dash-bootstrap-components-1.4.2rc1/landing-page.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-09 21:45:19.000000 dash-bootstrap-components-1.4.2rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-09 21:46:47.969700 dash-bootstrap-components-1.4.2rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-09 21:45:19.000000 dash-bootstrap-components-1.4.2rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:46:47.969700 dash-bootstrap-components-1.4.2rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-09 21:45:19.000000 dash-bootstrap-components-1.4.2rc1/tests/test_alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-09 21:45:19.000000 dash-bootstrap-components-1.4.2rc1/tests/test_components_as_props.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-07-09 21:45:19.000000 dash-bootstrap-components-1.4.2rc1/tests/test_navlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-09 21:45:19.000000 dash-bootstrap-components-1.4.2rc1/tests/test_popover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-09 21:45:19.000000 dash-bootstrap-components-1.4.2rc1/tests/test_positional_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-09 21:45:19.000000 dash-bootstrap-components-1.4.2rc1/tests/test_tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-09 21:45:19.000000 dash-bootstrap-components-1.4.2rc1/tests/test_version.py
```

### Comparing `dash-bootstrap-components-1.4.1rc2/LICENSE` & `dash-bootstrap-components-1.4.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/PKG-INFO` & `dash-bootstrap-components-1.4.2rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-bootstrap-components
-Version: 1.4.1rc2
+Version: 1.4.2rc1
 Summary: Bootstrap themed components for use in Plotly Dash
 Home-page: https://dash-bootstrap-components.opensource.faculty.ai/
 Author: Faculty
 Author-email: opensource@faculty.ai
 License: Apache Software License
 Project-URL: Bug Reports, https://github.com/facultyai/dash-bootstrap-components/issues
 Project-URL: Source, https://github.com/facultyai/dash-bootstrap-components/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dash-bootstrap-components Version: 1.4.1rc2
+Metadata-Version: 2.1 Name: dash-bootstrap-components Version: 1.4.2rc1
 Summary: Bootstrap themed components for use in Plotly Dash Home-page: https://
 dash-bootstrap-components.opensource.faculty.ai/ Author: Faculty Author-email:
 opensource@faculty.ai License: Apache Software License Project-URL: Bug
 Reports, https://github.com/facultyai/dash-bootstrap-components/issues Project-
 URL: Source, https://github.com/facultyai/dash-bootstrap-components/
 Classifier: Framework :: Dash Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python :: 3.7 Classifier:
```

### Comparing `dash-bootstrap-components-1.4.1rc2/README.md` & `dash-bootstrap-components-1.4.2rc1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -49,41 +49,14 @@
 You can also install _dash-bootstrap-components_ with `conda` through the
 conda-forge channel:
 
 ```sh
 conda install -c conda-forge dash-bootstrap-components
 ```
 
-### Dash for R
-
-You can now use _dash-bootstrap-components_ with Dash for R! To get started make sure you have the _devtools_ library installed
-
-```r
-install.packages("devtools")
-```
-
-You can then install _dash-bootstrap-components_ from the `r-release` branch of this repository.
-
-```r
-library(devtools)
-install_github('facultyai/dash-bootstrap-components@r-release')
-```
-
-Check out [the docs for more details](https://dash-bootstrap-components.opensource.faculty.ai/docs/quickstart)
-
-### Dash.jl
-
-You can also use _dash-bootstrap-components_ with Dash.jl! Install with
-
-```jl
-pkg> add DashBootstrapComponents
-```
-
-Check out [the docs for more details](https://dash-bootstrap-components.opensource.faculty.ai/docs/quickstart)
-
 ## Quick start
 
 To use _dash-bootstrap-components_ you must do two things:
 
 - Link a Bootstrap v5 compatible stylesheet
 - Incorporate _dash-bootstrap-components_ into your layout
```

#### html2text {}

```diff
@@ -8,29 +8,19 @@
 components for use with [Plotly Dash][dash-homepage], that makes it easier to
 build consistently styled Dash apps with complex, responsive layouts. ## Table
 of contents - [Installation](#installation) - [Quick start](#quick-start) -
 [Contributing](#contributing) - [Copyright and license](#copyright-and-license)
 ## Installation ### PyPI You can install _dash-bootstrap-components_ with
 `pip`: ```sh pip install dash-bootstrap-components ``` ### Anaconda You can
 also install _dash-bootstrap-components_ with `conda` through the conda-forge
-channel: ```sh conda install -c conda-forge dash-bootstrap-components ``` ###
-Dash for R You can now use _dash-bootstrap-components_ with Dash for R! To get
-started make sure you have the _devtools_ library installed ```r
-install.packages("devtools") ``` You can then install _dash-bootstrap-
-components_ from the `r-release` branch of this repository. ```r library
-(devtools) install_github('facultyai/dash-bootstrap-components@r-release') ```
-Check out [the docs for more details](https://dash-bootstrap-
-components.opensource.faculty.ai/docs/quickstart) ### Dash.jl You can also use
-_dash-bootstrap-components_ with Dash.jl! Install with ```jl pkg> add
-DashBootstrapComponents ``` Check out [the docs for more details](https://dash-
-bootstrap-components.opensource.faculty.ai/docs/quickstart) ## Quick start To
-use _dash-bootstrap-components_ you must do two things: - Link a Bootstrap v5
-compatible stylesheet - Incorporate _dash-bootstrap-components_ into your
-layout ### Linking a stylesheet _dash-bootstrap-components_ doesn't come with
-CSS included. This is to give you the freedom to use any Bootstrap v5
+channel: ```sh conda install -c conda-forge dash-bootstrap-components ``` ##
+Quick start To use _dash-bootstrap-components_ you must do two things: - Link a
+Bootstrap v5 compatible stylesheet - Incorporate _dash-bootstrap-components_
+into your layout ### Linking a stylesheet _dash-bootstrap-components_ doesn't
+come with CSS included. This is to give you the freedom to use any Bootstrap v5
 stylesheet of your choice. This means however that in order for the components
 to be styled properly, you must link to a stylesheet yourself. For convenience,
 links to [BootstrapCDN][bootstrapcdn] for each theme are available through the
 `themes` module, which can be used as follows: ```python import dash import
 dash_bootstrap_components as dbc app = dash.Dash(external_stylesheets=
 [dbc.themes.BOOTSTRAP]) ``` For more information on how to link local or
 external CSS, check out the [Dash documentation][dash-docs-external]. ### Build
```

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/__init__.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/__init__.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Accordion.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Accordion.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/AccordionItem.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/AccordionItem.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Alert.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Alert.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Badge.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Badge.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Breadcrumb.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Breadcrumb.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Button.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Button.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/ButtonGroup.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/ButtonGroup.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Card.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Card.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/CardBody.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/CardBody.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/CardFooter.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/CardFooter.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/CardGroup.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/CardGroup.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/CardHeader.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/CardHeader.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/CardImg.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/CardImg.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/CardImgOverlay.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/CardImgOverlay.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/CardLink.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/CardLink.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Carousel.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Carousel.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Checkbox.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Checkbox.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Checklist.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Checklist.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Col.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Col.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Collapse.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Collapse.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Container.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Container.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/DropdownMenu.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/DropdownMenu.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/DropdownMenuItem.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/DropdownMenuItem.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Fade.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Fade.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Form.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Form.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/FormFeedback.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/FormFeedback.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/FormFloating.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/FormFloating.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/FormText.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/FormText.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Input.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Input.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/InputGroup.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/InputGroup.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/InputGroupText.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/InputGroupText.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Label.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Label.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/ListGroup.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/ListGroup.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/ListGroupItem.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/ListGroupItem.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Modal.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Modal.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/ModalBody.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/ModalBody.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/ModalFooter.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/ModalFooter.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/ModalHeader.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/ModalHeader.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/ModalTitle.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/ModalTitle.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Nav.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Nav.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/NavItem.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/NavItem.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/NavLink.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/NavLink.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Navbar.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Navbar.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/NavbarBrand.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/NavbarBrand.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/NavbarSimple.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/NavbarSimple.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/NavbarToggler.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/NavbarToggler.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Offcanvas.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Offcanvas.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Pagination.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Pagination.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Placeholder.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Placeholder.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Popover.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Popover.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/PopoverBody.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/PopoverBody.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/PopoverHeader.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/PopoverHeader.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Progress.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Progress.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/RadioButton.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/RadioButton.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/RadioItems.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/RadioItems.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Row.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Row.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Select.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Select.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Spinner.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Spinner.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Stack.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Stack.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Switch.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Switch.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Tab.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Tab.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Table.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Table.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Tabs.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Tabs.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Textarea.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Textarea.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Toast.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Toast.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/Tooltip.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/Tooltip.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/__init__.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/__init__.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/dash_bootstrap_components.min.js` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/dash_bootstrap_components.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -2086,15 +2086,18 @@
                 p = t.style,
                 f = t.class_name,
                 g = t.className,
                 b = t.fade,
                 y = o(t, jt),
                 h = (0, i.useRef)(null);
             (0, i.useEffect)((function() {
-                a && (s ? h.current = setTimeout(v, a) : h.current && (clearTimeout(h.current), h.current = null))
+                return a && (s ? h.current = setTimeout(v, a) : h.current && (clearTimeout(h.current), h.current = null)),
+                    function() {
+                        return clearTimeout(h.current)
+                    }
             }), [s]);
             var v = function() {
                     u && u({
                         is_open: !1
                     })
                 },
                 _ = Nt.has(d);
```

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_components/metadata.json` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_components/metadata.json`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/_table.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/_table.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components/themes.py` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components/themes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 BOOTSTRAP = (
-    "https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/css/bootstrap.min.css"
+    "https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css"
 )
 
-GRID = "https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/css/bootstrap-grid.min.css"  # noqa
+GRID = "https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap-grid.min.css"  # noqa
 
-_BOOTSWATCH_BASE = "https://cdn.jsdelivr.net/npm/bootswatch@5.2.3/dist/"
+_BOOTSWATCH_BASE = "https://cdn.jsdelivr.net/npm/bootswatch@5.3.0/dist/"
 
 CERULEAN = _BOOTSWATCH_BASE + "cerulean/bootstrap.min.css"
 COSMO = _BOOTSWATCH_BASE + "cosmo/bootstrap.min.css"
 CYBORG = _BOOTSWATCH_BASE + "cyborg/bootstrap.min.css"
 DARKLY = _BOOTSWATCH_BASE + "darkly/bootstrap.min.css"
 FLATLY = _BOOTSWATCH_BASE + "flatly/bootstrap.min.css"
 JOURNAL = _BOOTSWATCH_BASE + "journal/bootstrap.min.css"
```

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components.egg-info/PKG-INFO` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-bootstrap-components
-Version: 1.4.1rc2
+Version: 1.4.2rc1
 Summary: Bootstrap themed components for use in Plotly Dash
 Home-page: https://dash-bootstrap-components.opensource.faculty.ai/
 Author: Faculty
 Author-email: opensource@faculty.ai
 License: Apache Software License
 Project-URL: Bug Reports, https://github.com/facultyai/dash-bootstrap-components/issues
 Project-URL: Source, https://github.com/facultyai/dash-bootstrap-components/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dash-bootstrap-components Version: 1.4.1rc2
+Metadata-Version: 2.1 Name: dash-bootstrap-components Version: 1.4.2rc1
 Summary: Bootstrap themed components for use in Plotly Dash Home-page: https://
 dash-bootstrap-components.opensource.faculty.ai/ Author: Faculty Author-email:
 opensource@faculty.ai License: Apache Software License Project-URL: Bug
 Reports, https://github.com/facultyai/dash-bootstrap-components/issues Project-
 URL: Source, https://github.com/facultyai/dash-bootstrap-components/
 Classifier: Framework :: Dash Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python :: 3.7 Classifier:
```

### Comparing `dash-bootstrap-components-1.4.1rc2/dash_bootstrap_components.egg-info/SOURCES.txt` & `dash-bootstrap-components-1.4.2rc1/dash_bootstrap_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/landing-page.md` & `dash-bootstrap-components-1.4.2rc1/landing-page.md`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/setup.cfg` & `dash-bootstrap-components-1.4.2rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/setup.py` & `dash-bootstrap-components-1.4.2rc1/setup.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/tests/test_components_as_props.py` & `dash-bootstrap-components-1.4.2rc1/tests/test_components_as_props.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/tests/test_navlink.py` & `dash-bootstrap-components-1.4.2rc1/tests/test_navlink.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/tests/test_popover.py` & `dash-bootstrap-components-1.4.2rc1/tests/test_popover.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/tests/test_positional_args.py` & `dash-bootstrap-components-1.4.2rc1/tests/test_positional_args.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.4.1rc2/tests/test_tooltip.py` & `dash-bootstrap-components-1.4.2rc1/tests/test_tooltip.py`

 * *Files identical despite different names*

