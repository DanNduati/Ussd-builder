<h1 align="center"><b>USSD menu builder</b></h1>

[![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://github.com/DanNduati/ussd-menu-builder)

## <b>Description</b>
In the course of creating USSD applications one of the biggest challenge I faced was handling navigation. Using conditionals presents the following challenges:
- With complex nested menus, conditionals quickly grow into messy spaghetti code. [case in point](https://github.com/DanNduati/Ussd-stkpush/blob/main/app/routers/ussd.py#L32)
- Having to write a conditional for every user input is not scalable

## <b>Inspiration</b>
Overall the conditionals approach is not it! In my search for a a better implementation I came across [this](https://github.com/habbes/ussd-menu-builder) node js ussd builder library that uses state machines to create USSD menus. A state is created for each menu. Each state has a unique name and a set of rules used to link to the other states based on the user input. So this is an attempt to implement a similar solution with Python.

## <b>License</b>
[![license](https://img.shields.io/github/license/mashape/apistatus.svg?style=for-the-badge)](LICENSE)