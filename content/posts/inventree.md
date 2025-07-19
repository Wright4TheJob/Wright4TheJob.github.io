+++
date = '2025-07-17T21:58:49-07:00'
draft =true
title = 'InvenTree and Data Flows'
+++

## Use Case
I often create assemblies with a significant number of unique parts, some of which I may have and others which need to be ordered. I've run ordering for engineering projects via Excel, and I know how quickly that becomes complex and almost un-trackable. Other than the additional time sunk into managing these Bills of Materials (BoMs), there are two forms of waste this creates:
1. **Overstocking**: Duplicate ordering of parts that may be on hand, but aren't known to be available.
2. **Delays**: If even a few small parts are missed in the initial round of ordering, the time delay can be anywhere from a few days to a week, depending on where parts are sourced from. This delays assembly, testing, and use of what is getting built.

## BoM Creation Trade-Offs
Creating the BoM for an assembly requires a non-trivial time investment. Part files must be created before assemblies can be listed, and sub-assemblies sometimes make the part tree deeper and more complex. The advantages, however, are that part statuses across the whole design tree can be checked, lead times automatically calculated when available from vendors, and costing can be easily updated. Ordering becomes trivial if in-stock quantites are up to date as well.
