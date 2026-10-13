# Print Envoy ZPL Developer Examples

Practical Zebra Programming Language examples for developers, consultants, warehouse teams, ERP implementations, and label-printing projects.

This repository provides reusable ZPL samples for text, barcodes, QR codes, warehouse labels, printer resolution testing, and multi-label workflows.

## Test ZPL Online

Use the **Print Envoy ZPL Visualizer** to preview, inspect, and troubleshoot ZPL directly in your browser.

**Open the ZPL Visualizer Tool**

https://printenvoy.com/zpl-visualizer-tool/

**Learn more about the ZPL Visualizer**

https://printenvoy.com/zpl-visualizer/

---

## Quick Start

1. Choose one of the ZPL examples below.
2. Open the `.zpl` file.
3. Copy the ZPL code.
4. Open the Print Envoy ZPL Visualizer.
5. Paste the ZPL into the editor.
6. Preview and inspect the rendered label.
7. Validate final output on the target printer before production use.

---

## ZPL Examples

| Example | Description | ZPL File |
|---|---|---|
| Basic Text Label | Simple text and field positioning example | [View ZPL](examples/basic-text/basic-text.zpl) |
| Code 128 Barcode | Code 128 barcode with human-readable text | [View ZPL](examples/barcodes/code128.zpl) |
| Code 39 Barcode | Code 39 barcode example | [View ZPL](examples/barcodes/code39.zpl) |
| UPC-A Barcode | UPC-A retail barcode example | [View ZPL](examples/barcodes/upc-a.zpl) |
| QR Code | QR code generated with ZPL | [View ZPL](examples/qr-code/qr-code.zpl) |
| Warehouse Location Label | Warehouse rack and location identification example | [View ZPL](examples/warehouse/location-label.zpl) |
| Inventory Label | Inventory item and barcode label example | [View ZPL](examples/warehouse/inventory-label.zpl) |
| Pallet Label | Larger pallet identification label | [View ZPL](examples/warehouse/pallet-label.zpl) |
| 203 DPI Example | Example designed around common 203 DPI printer dimensions | [View ZPL](examples/dpi/203-dpi-example.zpl) |
| 300 DPI Example | Example designed around common 300 DPI printer dimensions | [View ZPL](examples/dpi/300-dpi-example.zpl) |
| Multi-Label ZPL | Multiple `^XA` and `^XZ` label blocks in one ZPL source | [View ZPL](examples/multi-label/multi-label.zpl) |

---

## Example: Basic ZPL Label

```zpl
^XA
^PW609
^LL406
^FO60,70
^A0N,36,36
^FDPrint Envoy ZPL Example^FS
^FO60,130
^A0N,26,26
^FDHello from Zebra Programming Language^FS
^XZ
