## API Report File for "@fluentui/react-tabs"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts

import { IButtonProps } from 'office-ui-fabric-react';
import { IKeytipProps } from 'office-ui-fabric-react';
import { IRefObject } from '@uifabric/utilities';
import { IRenderFunction } from '@uifabric/utilities';
import { IStyle } from '@uifabric/styling';
import { IStyleFunctionOrObject } from '@uifabric/utilities';
import { ITheme } from '@uifabric/styling';
import * as React from 'react';

// @public (undocumented)
export interface IPivot {
    focus(): void;
}

// @public (undocumented)
export interface IPivotItemProps extends React.HTMLAttributes<HTMLDivElement> {
    alwaysRender?: boolean;
    ariaLabel?: string;
    componentRef?: IRefObject<{}>;
    headerButtonProps?: IButtonProps | {
        [key: string]: string | number | boolean;
    };
    headerText?: string;
    itemCount?: number | string;
    itemIcon?: string;
    itemKey?: string;
    keytipProps?: IKeytipProps;
    // @deprecated
    linkText?: string;
    onRenderItemLink?: IRenderFunction<IPivotItemProps>;
}

// @public (undocumented)
export interface IPivotProps extends React.HTMLAttributes<HTMLDivElement> {
    className?: string;
    componentRef?: React.RefObject<IPivot>;
    defaultSelectedKey?: string;
    getTabId?: (itemKey: string, index: number) => string;
    headersOnly?: boolean;
    linkFormat?: PivotLinkFormatType;
    linkSize?: PivotLinkSizeType;
    onLinkClick?: (item?: PivotItem, ev?: React.MouseEvent<HTMLElement>) => void;
    overflowBehavior?: 'none' | 'menu';
    selectedKey?: string | null;
    styles?: IStyleFunctionOrObject<IPivotStyleProps, IPivotStyles>;
    theme?: ITheme;
}

// @public (undocumented)
export type IPivotStyleProps = Required<Pick<IPivotProps, 'theme'>> & Pick<IPivotProps, 'className'> & Pick<IPivotProps, 'linkSize'> & Pick<IPivotProps, 'linkFormat'> & {
    linkIsSelected?: boolean;
};

// @public (undocumented)
export interface IPivotStyles {
    // (undocumented)
    count: IStyle;
    // (undocumented)
    icon: IStyle;
    // (undocumented)
    itemContainer?: IStyle;
    // (undocumented)
    link: IStyle;
    // (undocumented)
    linkContent: IStyle;
    // (undocumented)
    linkInMenu: IStyle;
    // (undocumented)
    linkIsSelected: IStyle;
    // (undocumented)
    overflowMenuButton: IStyle;
    root: IStyle;
    // (undocumented)
    text: IStyle;
}

// @public
export const Pivot: React.FunctionComponent<IPivotProps>;

// @public (undocumented)
export const PivotBase: React.FunctionComponent<IPivotProps>;

// @public (undocumented)
export class PivotItem extends React.Component<IPivotItemProps, {}> {
    constructor(props: IPivotItemProps);
    // (undocumented)
    render(): JSX.Element;
}

// @public @deprecated (undocumented)
export const enum PivotLinkFormat {
    links = "links",
    tabs = "tabs"
}

// @public
export type PivotLinkFormatType = 'links' | 'tabs';

// @public @deprecated (undocumented)
export const enum PivotLinkSize {
    large = "large",
    normal = "normal"
}

// @public
export type PivotLinkSizeType = 'normal' | 'large';


export * from "@fluentui/react-theme-provider";

// (No @packageDocumentation comment for this package)

```
