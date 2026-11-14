# SmartRetail - Project 4 (Retail Staff Assistant) - Group 04

## 1. Members
| Name | GitHub username |
|------|-----------------|
| Trần Kiều Oanh | kieuoanh-ally |
| Nguyễn Phước Vĩnh Huy | Jalter0602 |
| Võ An An | Tiso0229 |
| Huỳnh Gia Tuệ | giatue1604 |

Lecturer: vvvanthe

## 2. Problem (specification)
A C++17 command-line program that helps retail staff look up products, check stock, list promotions and total a shopping cart.

- **Input:** `products.csv`, `inventory.csv`, `promotions.csv` (`feedback.csv` for the extension) and commands typed on the keyboard.
- **Processing:** load CSV files into vectors of structs, skip invalid lines with a warning on cerr, search products by code or keyword, classify stock, pick the best promotion, compute the cart total with `long long`.
- **Output:** product details, stock status, promotions, cart lines and total. Stock is deducted in memory only after confirmation.

## 3. Build and run
```bash
g++ -std=c++17 -Wall -Wextra src/main.cpp -o bin/p4
./bin/p4 data/sample S001
```

## 4. Assumptions and limitations
- store_id defaults to S001 when not given.
- Stock is deducted in memory only; CSV files are never modified.
- Fields contain no commas and no Vietnamese diacritics.

## 5. What this project does NOT do
- Does not store card numbers, CVV or any payment data; it only prints accepted payment methods.
- Only reads and presents data; it does not write to the CSV files.
- Does not use classes, pointers, inheritance, map/set, exceptions or std::sort.

## 6. Task assignment table

| ID | Task | Function / file | Assignee | Reviewer | Flowchart | PR |
|----|------|-----------------|----------|----------|-----------|----|
| T01 | Repo skeleton | .gitignore, pull_request_template.md, README.md | Oanh | Huy | not needed | |
| T02 | Input Menu (3-5) | loadPromotions() | Huy | Oanh | yes | |
| T03 | Output (1) | searchProduct(), sortProducts(), findProduct() | Huy | Oanh | yes | |
| T04 | Input Menu (1-2) | loadProducts(), loadInventory() | An | Tuệ | yes | |
| T05 | Output (2) | checkInventory(), stockStatus() | An | Tuệ | yes | |
| T06 | Helper Function Calculator (4) | finalPrice(), bestPromotion(), cartTotal() | Tuệ | Huy | yes | |
| T07 | Output (3) | checkPromotion() | Tuệ | Huy | yes | |
| T08 | Output (4) | checkout(), confirm() | Oanh | An | yes | |
| T09 | Display Menu, Build Switch | showMenu(), toInt(), main() | Oanh | An | yes | |
| T10 | Slides | docs/slides.pdf | Oanh, Tuệ | An | not needed | |
| T11 | Architecture | docs/architecture.md | An, Huy | Oanh | not needed | |
| T12 | Test cases | tests/test_cases.md | Tuệ | An | not needed | |
| T13 | Demo | | An | Tuệ, Huy | not needed | |

## 7. AI declaration and references
<!-- Which tool, for what, which part of the code -->
