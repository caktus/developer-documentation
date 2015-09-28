Supported Browsers and Devices
##############################

There are hundreds of browsers that have been released over the course of the Web’s lifetime. There are thousands of distinct versions between all of these different browsers. We will not be testing every project across thousands of individual test browsers, so we need to narrow down the selection to a concise set of browser versions that represent the largest possible swath of the target user base.

Keep in mind that depending on the project the target user base will be made of people from different demographics, from different areas, with distinct technological patterns. The best set of browser versions to test may differ between projects based on the understanding of this user base.

The rule of thumb is: the latest two versions of Major Browsers. There are some special cases related to mobile browsers.

Major Browsers
==============

We consider the following vendors to produce “Major Browsers” for the purposes of determining a default set of support browsers.

- Google (Chrome)
- Mozilla (Firefox)
- Microsoft (Internet Explorer, Edge)
- Apple (Safari, Mobile Safari)

Grading System
==============

We will rate browsers and devices by a simple grading system. This helps to
categorize the approach to support for each browser. As any release ages, its
grade will be reduced.

=====   ========================================================================================
Grade   Level of Support Offered
=====   ========================================================================================
A       Supported by default in all new projects.
B       Supported by default, but allowed to present degraded experiences based on unsupported features.
C       Not supported by default. If required in a project, additional time must be estimated. Support may be degraded.
D       Not supported by default. Will strongly discourage support at client request.
=====   ========================================================================================

Current Grade Chart
===================

Browsers
--------

=========   ===================     ===========     =====
Vendor      Browser                 Version(s)      Grade
=========   ===================     ===========     =====
Google      Chrome                  44              **A**
Google      Chrome                  43              **A**
Mozilla     Firefox                 39              **A**
Mozilla     Firefox                 38              **A**
Apple       Safari                  8               **A**
Apple       Safari                  7               B
Apple       Safari Mobile           8               **A**
Google      Chrome for Android      42              B
Google      Android Browser         4.2-4.3         C
Google      Android Browser         2.3-4.1         C
Microsoft   Edge                    1               **A**
Microsoft   Internet Explorer       11              **A**
Microsoft   Internet Explorer       10              **B**
Microsoft   Internet Explorer       9               C
Microsoft   Internet Explorer       8 and below     D
=========   ===================     ===========     =====

Target Layouts
==============

Alongside our starting set of supported browsers every project begins with a starting set of
target layouts to be both designed and developed for. We do not want to prescribe a concrete set of
breakpoints for Desktop, Mobile, and Tablet devices and possibly requiring multiple breakpoints for
some or all of those device types.

Instead, every project should include at least one target layout for Desktop browsers and one
target layout for Mobile browsers. The layout for mobile browsers should also apply to tablet
devices, unless there is are specific components in the layout that have to be lost on mobile but
are important enough to warrant extra layouts to add on tablets. This should be carefully
considered.

Down to specific breakpoints, it is recommended they be considered on a per-component basis. Rather
than defining global breakpoints for the entire site at some specific screen width, it would be
preferable to look at each component being built and outline the breakpoints that make sense for it,
starting at the highest level components like a top nav bar, site and page headers, and the site
footer. 

Update Policy
=============

This policy and the gradings should be reviewed at least quarterly by QA or development, or when
beginning a new project and commiting to the support levels defined by this document.
