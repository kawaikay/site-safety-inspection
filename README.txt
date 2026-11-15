Site Safety Inspection PWA v4

Added databanks:
- Foundation & Piling Works: FP1-FP20
- Excavation & Lateral Support (ELS): EL1-EL20

The additions consolidate recurring observations from the supplied CHR weekly safety reports (March-August 2023), including plant stability and visibility, piling pins and guards, casings/drilling-rod wedging, lifting points and gear, Form 4, permit-to-dig, slope stability/protection, guardrails, access, openings, water control, temporary services and public protection.

PDF enhancement:
- Every FAIL item is summarized under General Safety Issues Identified.
- Only selected PASS/FAIL/N/A items are shown.
- Photos remain offline, include a permanent timestamp overlay, and appear under the selected item.

Deployment:
Upload all extracted files to the existing GitHub repository root and replace files with the same names. GitHub Pages will redeploy automatically. The service-worker cache is v4.

DATABANK EXTENSION v5
Included additional Weekly Safety Inspection Reports dated 9 Aug 2023 to 6 Nov 2023.
New items FP21-FP30, EL21-EL27, D5-D6, R4 and W6 cover load indicators/alarms, lifting fatal zones, hook and latch condition, SWL identification, wire-sling storage, mixed-load lifting, plant isolation, hose integrity, operator refresher training, scaffold/access inspection, toe boards, checking-point covers, stagnant water, haul-road routing, securely fixed barriers, sump-pit lifesaving equipment, lifting/scaffold documentation, adverse weather and unattended flame cutting.

DATABANK ORGANISATION v6
- Foundation & Piling Works and Excavation & Lateral Support (ELS) are no longer separate Main Categories.
- All additional controls derived from the supplied CHR WSI reports have been allocated into the existing Main Categories: Lifting Operations, Piling Operations, PPE, Documentation, Excavation & Slope, Access & Egress, Falling Objects Protection, Housekeeping, Electrical Safety and Site Rules.
- Existing category names and mobile navigation are retained.


DATABANK CONSOLIDATION v7
Semantically overlapping items were merged while preserving the more complete control wording. Separate controls were retained where inspection evidence differs, such as extinguisher location versus certification, or access versus edge protection.

GENERAL HYGIENE CONDITION v8
Added General Hygiene Condition / 一般衛生情況 as a Main Category with GH1-GH12 covering cleanliness, waste, food waste, mosquito breeding, pest control, toilets/washing facilities, hand washing, drinking water, welfare areas, drainage and dust/mud hygiene.
FAIL items automatically feed the existing General Safety Issues Identified section using hygiene risk groups such as Cleanliness, Waste, Pest Control, Sanitary Facilities, Drinking Water, Welfare Facilities, Drainage and Dust/Mud.


ARUP PAGE MARK v9
- Added a red ARUP text mark at the top-right of every printed PDF page.
- The implementation uses a fixed print element so the browser print engine repeats it on each A4 page.
- This is a text reproduction matching the supplied visual reference, not an embedded official logo asset.


PHOTO DELETE FUNCTION v10
- Each stored photo thumbnail now has a red X delete button.
- The user is asked to confirm before deletion.
- Deletion removes the photo from IndexedDB, so the removed photo will not appear in the offline PDF.
- Users can immediately retake a clearer photo using Take Photo.


v11 REPORT / PHOTO OPTIMISATION
- Changed Inspector label to RSS Representative / 駐地工程師代表 in the PWA input form.
- Changed PDF report field from Inspector to RSS Representative.
- Reduced stored photo long edge from 1800 px to 1280 px.
- Reduced JPEG quality from 88% to 70% to reduce IndexedDB storage and PDF file size while retaining sufficient visual detail for normal safety observations.
- Timestamp, inspection number and item number remain burned into each stored image.


v12 PHOTO REPORT LAYOUT
- Removed the separate large Photo Taken date/time caption below photos in the PDF report.
- Date/time remains permanently burned into the lower part of each stored photo, together with Item ID and Inspection ID.
- The small date/time beneath the thumbnail inside the PWA remains available for checking before report export.

v13 PHOTO THUMBNAIL TIMESTAMP
- Increased the timestamp displayed below each photo thumbnail in the PWA inspection screen to 14 px, bold, dark text.
- Added 6 px spacing above the timestamp for readability on mobile phones.
- PDF layout is unchanged: the separate large timestamp below PDF photos remains removed because date/time is already burned into each photo.
