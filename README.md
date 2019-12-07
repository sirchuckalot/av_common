av_common
======

av_common is a set of constants and function that can be used for anyone implementing a Avalon-compatible device

Files
-----

- av_common_params.v : Contains Avalon constants
- av_common.v : Contains Avalon utility functions

Functions
---------

- get_cycle_type(cti) : Returns 1 for burst cycles and 0 for classic cycles
- av_is_last(cti) : Returns 1 for last cycle of a burst or single cycle accesses. Returns 0 if more cycles are expected
- av_next_adr(adr, cti, bte, dw) : Calculates the next address for incrementing burst accesses. Returns adr for other accesses
