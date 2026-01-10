# eBay UK TCG Fee Calculator

A static site for quick eBay fee calculation, specifically designed for UK sellers in the Collectables category (Trading Card Games).

## Features

### Account Types

- **Private Seller** — Uses eBay's Buyer Protection fee structure (tiered percentage)
- **Business Seller** — Uses Final Value Fee + Regulatory Operating Fee + Fixed Fee

### Fee Calculations

#### Private Seller (Buyer Protection)
| Price Range | Fee Rate |
|-------------|----------|
| Flat fee | £0.10 per item |
| £0 – £20 | 7% |
| £20 – £300 | 4% |
| £300 – £4,000 | 2% |
| £4,000+ | No additional fee |

#### Business Seller
| Fee Type | Rate |
|----------|------|
| Final Value Fee | 10.9% |
| Regulatory Operating Fee | 0.35% |
| Fixed Fee (orders ≤£10) | £0.10 per item |
| Fixed Fee (orders >£10) | £0.30 per item |
| Minimum Fee | £0.05 |
| VAT on Fees | 20% |
| Top-Rated Seller Discount | 10% off FVF |

### Postage Options

Automatically selects Royal Mail postage based on item price, or manually choose:

| Service | Cost | Auto-Selected For |
|---------|------|-------------------|
| 2nd Class | £0.87 | Items under £20 |
| 1st Class | £1.70 | — |
| Tracked 48 | £2.75 | Items £20 – £150 |
| Tracked 24 | £3.65 | — |
| Special Delivery (1pm) | £8.75 | Items £150+ |

*Auto Postage is based on cheapest fully insured service for order value. Postage rates assume letter-size packaging.*

### Advanced Options

- **Free Postage Toggle** — Calculate with postage included in item price or charged separately
- **Postage Type Selection** — Auto-select based on price or manually choose
- **Top-Rated Seller** (Business only) — Apply 10% discount on Final Value Fee
- **Include VAT on Fees** (Business only) — Add 20% VAT to eBay fees

### Results Breakdown

- Itemized eBay fees with sub-breakdowns for business sellers
- Postage cost (when applicable)
- **"You Keep"** — Final amount after all deductions

## Usage

Simply open `index.html` in any modern browser. No build step or server required.

## Disclaimer

Fee calculations are estimates and may vary. Only works for UK eBay Collectables category. Always check [eBay's official fee structure](https://www.ebay.co.uk/help/selling/fees-credits-invoices/selling-fees?id=4822) for the most up-to-date information.
