# Yandex Business YML Feed for KM STUDIO

## Overview

This repository contains an enhanced YML feed for uploading massage services to Yandex Business advertising platform.

## Files

- `yandex_business_feed.yml` — Enhanced YML feed ready for Yandex Business
- `km_studio_massages_yml_min.xml` — Original minimal feed
- `ИНСТРУКЦИЯ_YML_FEED.md` — Detailed instructions in Russian
- `README.md` — This file

## Key Features

✅ Full compatibility with Yandex Business requirements  
✅ Extended category structure for better organization  
✅ Additional parameters for improved visibility  
✅ UTM tags for tracking campaign effectiveness  
✅ Vendor codes for analytics  
✅ Old prices to display discounts  
✅ Detailed descriptions with duration and features  

## Quick Start

1. **Update contact information** in `yandex_business_feed.yml`:
   - Phone number
   - Email address

2. **Add real image URLs** for all services (replace placeholder URLs)

3. **Verify prices and availability** are up to date

4. **Upload the file** to your server (e.g., `https://krismass.ru/feeds/yandex_business_feed.yml`)

5. **Import to Yandex Business**:
   - Go to https://business.yandex.ru/
   - Navigate to "Products and Services"
   - Click "Import" → "YML File"
   - Enter your feed URL
   - Click "Upload"

## Feed Structure

### Shop Information
- Name, company, URL
- Phone and email
- Currency (RUB)

### Categories
- Main: Массажи (Massages)
- Sub-categories: Relaxation, Therapeutic, Cosmetic

### Offers (18 total)
Each offer includes:
- Unique ID and URL with UTM tags
- Price (with optional old price for discounts)
- Category assignment
- High-quality images (to be added)
- Vendor and vendor code
- Detailed description
- Service parameters (duration, location, type)
- Delivery options (pickup/in-store)

## Branches

Services are available at two locations:
- **Юности 2** (Yunosti 2) — 9 services
- **Весенняя** (Vesennyaya) — 9 services

## Service Types

1. **Relaxing Massages**
   - General relaxing full body massage
   - Deep relaxation full body massage (90 min)

2. **Therapeutic Massages**
   - Classic body massage
   - Back and neck massage

3. **Cosmetic Massages**
   - Body contouring massage
   - Anti-cellulite massage
   - Lymphatic drainage massage
   - Honey massage
   - Salt massage

## Before Uploading

### Required Updates

1. **Contact Information**
   ```xml
   <phone>+7 (XXX) XXX-XX-XX</phone>  <!-- Update this -->
   <email>info@krismass.ru</email>    <!-- Verify this -->
   ```

2. **Image URLs**
   ```xml
   <picture>https://krismass.ru/images/services/relax-massage.jpg</picture>
   ```
   
   Image requirements:
   - Format: JPG or PNG
   - Size: minimum 300×300 px, recommended 600×600 px or larger
   - Quality: high, no watermarks
   - Content: must match the service

### Validation

Test your feed before uploading:
- Yandex Webmaster: https://webmaster.yandex.ru/tools/market-feed/
- Check for XML syntax errors
- Verify all URLs are accessible
- Ensure images load correctly

## UTM Tracking

All URLs include UTM parameters for analytics:
- `utm_source=yandex_business`
- `utm_medium=import`
- `utm_campaign=products`
- `utm_branch=yunost` or `vesennyaya`
- `utm_service=service_name`

Use these in Yandex.Metrica to track campaign performance.

## Auto-Updates

Once set up, Yandex Business will automatically check your feed (usually daily):
1. Update the file on your server when prices or services change
2. Changes will be pulled automatically on the next check
3. No manual re-import needed

## Support

- Yandex Business Documentation: https://yandex.ru/support/business/
- YML Format Reference: https://yandex.ru/support/partnermarket/export/yml.html

## Version

- **Created**: October 29, 2025
- **Version**: 1.0
- **Format**: YML (Yandex Market Language)
- **Services**: 18 massage offerings across 2 locations
