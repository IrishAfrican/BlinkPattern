# BlinkPattern
Arduino library to generate complex blink patterns

Usage:
* Create object: BlinkPattern bp();
* Set pattern e.g. to flash once: bp.setPattern(BlinkPattern::Flash1);
* Or e.g. to blink slowly: bp.setPattern(BlinkPattern::Blink8);
* In timer or periodically: if(bp.nextState()) TURN_LED_ON else TURN_LED_OFF;
* To check if new pattern already started: if(bp.patternStarted()) ...