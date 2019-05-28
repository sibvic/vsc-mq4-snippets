# Profit Robots MQ4 code snippets for Visual Studio Code

## Indicators

### ichimoku

Translates into

    double ichValue = iIchimoku(_Symbol, _Period, tenkan_sen, kijun_sen, senkoi_span_b, (MODE_TENKANSEN,MODE_KIJUNSEN,MODE_SENKOUSPANA,MODE_SENKOUSPANB,MODE_CHIKOUSPAN), pos);

TODO: stochastic, averages, averagesOnArray, wpr, createArrowStream, createStream, createInternalStream, averagesTypeParam

### checkCustomIndicator

Check wether the custom indicator installed in the system. Should be used in the OnInit function.

Translates into

    double temp = iCustom(NULL, 0, "indicator", 0, 0);
    if (GetLastError() == ERR_INDICATOR_CANNOT_LOAD)
    {
       Alert("Please, install the 'indicator' indicator");
       return INIT_FAILED;
    }

## Code snippets for other platforms

* [FXTS2 Lua](https://github.com/sibvic/vsc-indicore)

## Donations gratefully accepted.

* [Donate via Paypal](https://paypal.me/sibvic)