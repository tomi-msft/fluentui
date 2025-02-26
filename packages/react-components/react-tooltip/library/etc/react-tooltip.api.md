## API Report File for "@fluentui/react-tooltip"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts

import type { ComponentProps } from '@fluentui/react-utilities';
import type { ComponentState } from '@fluentui/react-utilities';
import type { PortalProps } from '@fluentui/react-portal';
import type { PositioningShorthand } from '@fluentui/react-positioning';
import * as React_2 from 'react';
import type { Slot } from '@fluentui/react-utilities';
import type { SlotClassNames } from '@fluentui/react-utilities';
import type { TriggerProps } from '@fluentui/react-utilities';

// @public
export type OnVisibleChangeData = {
    visible: boolean;
    documentKeyboardEvent?: KeyboardEvent;
};

// @public
export const renderTooltip_unstable: (state: TooltipState) => JSX.Element;

// @public
export const Tooltip: React_2.FC<TooltipProps>;

// @public (undocumented)
export const tooltipClassNames: SlotClassNames<TooltipSlots>;

// @public
export type TooltipProps = ComponentProps<TooltipSlots> & TriggerProps<TooltipTriggerProps> & Pick<PortalProps, 'mountNode'> & {
    appearance?: 'normal' | 'inverted';
    hideDelay?: number;
    onVisibleChange?: (event: React_2.PointerEvent<HTMLElement> | React_2.FocusEvent<HTMLElement> | undefined, data: OnVisibleChangeData) => void;
    positioning?: PositioningShorthand;
    relationship: 'label' | 'description' | 'inaccessible';
    showDelay?: number;
    visible?: boolean;
    withArrow?: boolean;
};

// @public
export type TooltipSlots = {
    content: NonNullable<Slot<'div'>>;
};

// @public
export type TooltipState = ComponentState<TooltipSlots> & Pick<TooltipProps, 'mountNode' | 'relationship'> & Required<Pick<TooltipProps, 'appearance' | 'hideDelay' | 'positioning' | 'showDelay' | 'visible' | 'withArrow'>> & {
    children?: React_2.ReactElement | null;
    shouldRenderTooltip?: boolean;
    arrowRef?: React_2.Ref<HTMLDivElement>;
    arrowClassName?: string;
};

// @public
export type TooltipTriggerProps = {
    ref?: React_2.Ref<unknown>;
} & Pick<React_2.HTMLAttributes<HTMLElement>, 'aria-describedby' | 'aria-label' | 'aria-labelledby' | 'onBlur' | 'onFocus' | 'onPointerEnter' | 'onPointerLeave' | 'aria-haspopup' | 'aria-expanded'>;

// @public
export const useTooltip_unstable: (props: TooltipProps) => TooltipState;

// @public
export const useTooltipStyles_unstable: (state: TooltipState) => TooltipState;

// (No @packageDocumentation comment for this package)

```
