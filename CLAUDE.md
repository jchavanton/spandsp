We did not capture source of the error T30_ERR_NORESSUPPORT

When we compare something working with a failed negociation, we are missing something, can we log all the possible conditions that would result in 
T30_ERR_NORESSUPPORT


Working logs:
2026-01-26 21:59:06.610096 97.37% [WARNING] mod_spandsp_fax.c:302 WARNING T.30 Negotiated resolution: 8040 x 7700 pixels/meter (current_page_resolution=2)
2026-01-26 21:59:06.610096 97.37% [WARNING] mod_spandsp_fax.c:302 WARNING T.30   Image resolution in file: 8031 x 7716 pixels/meter
2026-01-26 21:59:06.610096 97.37% [WARNING] mod_spandsp_fax.c:302 WARNING T.30   Mutual bilevel resolutions: R8xSTD(~98x98dpi), R8xFINE(~98x196dpi), R8xSUPERFINE(~98x392dpi), R16xSUPERFINE(~196x392dpi), 200x100dpi, 200x200dpi, 200x400dpi, 400x400dpi
2026-01-26 21:59:06.610096 97.37% [WARNING] mod_spandsp_fax.c:302 WARNING T.30   Mutual colour resolutions: none
Failes logs:
2026-01-27 14:35:34.570094 95.40% [WARNING] mod_spandsp_fax.c:302 WARNING T.30 RESOLUTION NEGOTIATION FAILED: Cannot negotiate an image resolution
2026-01-27 14:35:34.570094 95.40% [WARNING] mod_spandsp_fax.c:302 WARNING T.30   Image resolution in file: 8031 x 7716 pixels/meter
2026-01-27 14:35:34.570094 95.40% [WARNING] mod_spandsp_fax.c:302 WARNING T.30   Mutual bilevel resolutions supported: R8xSTD(~98x98dpi), R8xFINE(~98x196dpi), R8xSUPERFINE(~98x392dpi), R16xSUPERFINE(~196x392dpi), 200x100dpi, 200x200dpi, 200x400dpi, 400x400dpi
2026-01-27 14:35:34.570094 95.40% [WARNING] mod_spandsp_fax.c:302 WARNING T.30   Mutual colour resolutions supported: none
2026-01-27 14:35:34.570094 95.40% [WARNING] mod_spandsp_fax.c:302 WARNING T.30   Suggestion: Resize image to one of the mutually supported resolutions
