## API Report File for "react-redux"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts

import { Action } from 'redux';
import { AnyAction } from 'redux';
import { ClassAttributes } from 'react';
import { Component } from 'react';
import { ComponentClass } from 'react';
import { ComponentType } from 'react';
import { Context } from 'react';
import { Dispatch } from 'redux';
import hoistNonReactStatics = require('hoist-non-react-statics');
import { NamedExoticComponent } from 'react';
import { Store } from 'redux';

// @public (undocumented)
export type AdvancedComponentDecorator<TProps, TOwnProps> =
(component: ComponentType<TProps>) => NamedExoticComponent<TOwnProps>;

// @public (undocumented)
export type AnyIfEmpty<T extends object> = keyof T extends never ? any : T;

// @public
export function batch(cb: () => void): void;

// @public
export interface Connect<DefaultState = DefaultRootState> {
    // tslint:disable:no-unnecessary-generics
    // (undocumented)
    (): InferableComponentEnhancer<DispatchProp>;

    // (undocumented)
    <TStateProps = {}, no_dispatch = {}, TOwnProps = {}, State = DefaultState>(
    mapStateToProps: MapStateToPropsParam<TStateProps, TOwnProps, State>
    ): InferableComponentEnhancerWithProps<TStateProps & DispatchProp, TOwnProps>;

    // (undocumented)
    <no_state = {}, TDispatchProps = {}, TOwnProps = {}>(
    mapStateToProps: null | undefined,
    mapDispatchToProps: MapDispatchToPropsNonObject<TDispatchProps, TOwnProps>
    ): InferableComponentEnhancerWithProps<TDispatchProps, TOwnProps>;

    // (undocumented)
    <no_state = {}, TDispatchProps = {}, TOwnProps = {}>(
    mapStateToProps: null | undefined,
    mapDispatchToProps: MapDispatchToPropsParam<TDispatchProps, TOwnProps>,
    ): InferableComponentEnhancerWithProps<
    ResolveThunks<TDispatchProps>,
    TOwnProps
    >;

    // (undocumented)
    <TStateProps = {}, TDispatchProps = {}, TOwnProps = {}, State = DefaultState>(
    mapStateToProps: MapStateToPropsParam<TStateProps, TOwnProps, State>,
    mapDispatchToProps: MapDispatchToPropsNonObject<TDispatchProps, TOwnProps>
    ): InferableComponentEnhancerWithProps<TStateProps & TDispatchProps, TOwnProps>;

    // (undocumented)
    <TStateProps = {}, TDispatchProps = {}, TOwnProps = {}, State = DefaultState>(
    mapStateToProps: MapStateToPropsParam<TStateProps, TOwnProps, State>,
    mapDispatchToProps: MapDispatchToPropsParam<TDispatchProps, TOwnProps>,
    ): InferableComponentEnhancerWithProps<
    TStateProps & ResolveThunks<TDispatchProps>,
    TOwnProps
    >;

    // (undocumented)
    <no_state = {}, no_dispatch = {}, TOwnProps = {}, TMergedProps = {}>(
    mapStateToProps: null | undefined,
    mapDispatchToProps: null | undefined,
    mergeProps: MergeProps<undefined, undefined, TOwnProps, TMergedProps>,
    ): InferableComponentEnhancerWithProps<TMergedProps, TOwnProps>;

    // (undocumented)
    <TStateProps = {}, no_dispatch = {}, TOwnProps = {}, TMergedProps = {}, State = DefaultState>(
    mapStateToProps: MapStateToPropsParam<TStateProps, TOwnProps, State>,
    mapDispatchToProps: null | undefined,
    mergeProps: MergeProps<TStateProps, undefined, TOwnProps, TMergedProps>,
    ): InferableComponentEnhancerWithProps<TMergedProps, TOwnProps>;

    // (undocumented)
    <no_state = {}, TDispatchProps = {}, TOwnProps = {}, TMergedProps = {}>(
    mapStateToProps: null | undefined,
    mapDispatchToProps: MapDispatchToPropsParam<TDispatchProps, TOwnProps>,
    mergeProps: MergeProps<undefined, TDispatchProps, TOwnProps, TMergedProps>,
    ): InferableComponentEnhancerWithProps<TMergedProps, TOwnProps>;

    // (undocumented)
    <TStateProps = {}, no_dispatch = {}, TOwnProps = {}, State = DefaultState>(
    mapStateToProps: MapStateToPropsParam<TStateProps, TOwnProps, State>,
    mapDispatchToProps: null | undefined,
    mergeProps: null | undefined,
    options: Options<State, TStateProps, TOwnProps>
    ): InferableComponentEnhancerWithProps<DispatchProp & TStateProps, TOwnProps>;

    // (undocumented)
    <TStateProps = {}, TDispatchProps = {}, TOwnProps = {}>(
    mapStateToProps: null | undefined,
    mapDispatchToProps: MapDispatchToPropsNonObject<TDispatchProps, TOwnProps>,
    mergeProps: null | undefined,
    options: Options<{}, TStateProps, TOwnProps>
    ): InferableComponentEnhancerWithProps<TDispatchProps, TOwnProps>;

    // (undocumented)
    <TStateProps = {}, TDispatchProps = {}, TOwnProps = {}>(
    mapStateToProps: null | undefined,
    mapDispatchToProps: MapDispatchToPropsParam<TDispatchProps, TOwnProps>,
    mergeProps: null | undefined,
    options: Options<{}, TStateProps, TOwnProps>
    ): InferableComponentEnhancerWithProps<
    ResolveThunks<TDispatchProps>,
    TOwnProps
    >;

    // (undocumented)
    <TStateProps = {}, TDispatchProps = {}, TOwnProps = {}, State = DefaultState>(
    mapStateToProps: MapStateToPropsParam<TStateProps, TOwnProps, State>,
    mapDispatchToProps: MapDispatchToPropsNonObject<TDispatchProps, TOwnProps>,
    mergeProps: null | undefined,
    options: Options<State, TStateProps, TOwnProps>
    ): InferableComponentEnhancerWithProps<TStateProps & TDispatchProps, TOwnProps>;

    // (undocumented)
    <TStateProps = {}, TDispatchProps = {}, TOwnProps = {}, State = DefaultState>(
    mapStateToProps: MapStateToPropsParam<TStateProps, TOwnProps, State>,
    mapDispatchToProps: MapDispatchToPropsParam<TDispatchProps, TOwnProps>,
    mergeProps: null | undefined,
    options: Options<State, TStateProps, TOwnProps>
    ): InferableComponentEnhancerWithProps<
    TStateProps & ResolveThunks<TDispatchProps>,
    TOwnProps
    >;

    // (undocumented)
    <TStateProps = {}, TDispatchProps = {}, TOwnProps = {}, TMergedProps = {}, State = DefaultState>(
    mapStateToProps: MapStateToPropsParam<TStateProps, TOwnProps, State>,
    mapDispatchToProps: MapDispatchToPropsParam<TDispatchProps, TOwnProps>,
    mergeProps: MergeProps<TStateProps, TDispatchProps, TOwnProps, TMergedProps>,
    options?: Options<State, TStateProps, TOwnProps, TMergedProps>
    ): InferableComponentEnhancerWithProps<TMergedProps, TOwnProps>;
    // tslint:enable:no-unnecessary-generics
}

// @public
export const connect: Connect;

// @public
export function connectAdvanced<S, TProps, TOwnProps, TFactoryOptions = {}>(
// tslint:disable-next-line no-unnecessary-generics
selectorFactory: SelectorFactory<S, TProps, TOwnProps, TFactoryOptions>,
connectOptions?: ConnectOptions & TFactoryOptions
): AdvancedComponentDecorator<TProps, TOwnProps>;

// @public (undocumented)
export type ConnectedComponent<
C extends ComponentType<any>,
P
> = NamedExoticComponent<JSX.LibraryManagedAttributes<C, P>> & hoistNonReactStatics.NonReactStatics<C> & {
    WrappedComponent: C;
};

// @public
export type ConnectedProps<TConnector> =
TConnector extends InferableComponentEnhancerWithProps<infer TInjectedProps, any>
? unknown extends TInjectedProps
? TConnector extends InferableComponentEnhancer<infer TInjectedProps>
? TInjectedProps
: never
: TInjectedProps
: never;

// @public (undocumented)
export interface ConnectOptions {
    context?: Context<ReactReduxContextValue>;
    getDisplayName?: (componentName: string) => string;
    methodName?: string;
    renderCountProp?: string;
    shouldHandleStateChanges?: boolean;
    storeKey?: string;
    // @deprecated (undocumented)
    withRef?: boolean;
}

// @public
export function createDispatchHook<S = RootStateOrAny, A extends Action = AnyAction>(
context?: Context<ReactReduxContextValue<S, A>>,
): () => Dispatch<A>;

// @public
export function createSelectorHook<S = RootStateOrAny, A extends Action = AnyAction>(
context?: Context<ReactReduxContextValue<S, A>>,
): <Selected extends unknown>(
selector: (state: S) => Selected,
equalityFn?: (previous: Selected, next: Selected) => boolean,
) => Selected;

// @public
export function createStoreHook<S = RootStateOrAny, A extends Action = AnyAction>(
context?: Context<ReactReduxContextValue<S, A>>,
): () => Store<S, A>;

// @public
export interface DefaultRootState {}

// @public (undocumented)
export interface DispatchProp<A extends Action = AnyAction> {
    // (undocumented)
    dispatch: Dispatch<A>;
}

// @public (undocumented)
export type DistributiveOmit<T, K extends keyof T> = T extends unknown ? Omit_2<T, K> : never;

// @public (undocumented)
export type GetProps<C> = C extends ComponentType<infer P>
? C extends ComponentClass<P> ? ClassAttributes<InstanceType<C>> & P : P
: never;

// @public (undocumented)
export type HandleThunkActionCreator<TActionCreator> =
TActionCreator extends (...args: any[]) => any
? InferThunkActionCreatorType<TActionCreator>
: TActionCreator;

// @public (undocumented)
export type InferableComponentEnhancer<TInjectedProps> =
InferableComponentEnhancerWithProps<TInjectedProps, {}>;

// @public (undocumented)
export type InferableComponentEnhancerWithProps<TInjectedProps, TNeedsProps> =
<C extends ComponentType<Matching<TInjectedProps, GetProps<C>>>>(
component: C
) => ConnectedComponent<C, DistributiveOmit<GetProps<C>, keyof Shared<TInjectedProps, GetProps<C>>> & TNeedsProps>;

// @public (undocumented)
export type InferThunkActionCreatorType<TActionCreator extends (...args: any[]) => any> =
TActionCreator extends (...args: infer TParams) => (...args: any[]) => infer TReturn
? (...args: TParams) => TReturn
: TActionCreator;

// @public (undocumented)
export type MapDispatchToProps<TDispatchProps, TOwnProps> =
MapDispatchToPropsFunction<TDispatchProps, TOwnProps> | TDispatchProps;

// @public (undocumented)
export type MapDispatchToPropsFactory<TDispatchProps, TOwnProps> =
(dispatch: Dispatch<Action>, ownProps: TOwnProps) => MapDispatchToPropsFunction<TDispatchProps, TOwnProps>;

// @public (undocumented)
export type MapDispatchToPropsFunction<TDispatchProps, TOwnProps> =
(dispatch: Dispatch<Action>, ownProps: TOwnProps) => TDispatchProps;

// @public (undocumented)
export type MapDispatchToPropsNonObject<TDispatchProps, TOwnProps> = MapDispatchToPropsFactory<TDispatchProps, TOwnProps> | MapDispatchToPropsFunction<TDispatchProps, TOwnProps>;

// @public (undocumented)
export type MapDispatchToPropsParam<TDispatchProps, TOwnProps> = MapDispatchToPropsFactory<TDispatchProps, TOwnProps> | MapDispatchToProps<TDispatchProps, TOwnProps>;

// @public (undocumented)
export type MapStateToProps<TStateProps, TOwnProps, State = DefaultRootState> =
(state: State, ownProps: TOwnProps) => TStateProps;

// @public (undocumented)
export type MapStateToPropsFactory<TStateProps, TOwnProps, State = DefaultRootState> =
(initialState: State, ownProps: TOwnProps) => MapStateToProps<TStateProps, TOwnProps, State>;

// @public (undocumented)
export type MapStateToPropsParam<TStateProps, TOwnProps, State = DefaultRootState> =
MapStateToPropsFactory<TStateProps, TOwnProps, State> | MapStateToProps<TStateProps, TOwnProps, State> | null | undefined;

// @public
export type Matching<InjectedProps, DecorationTargetProps> = {
    [P in keyof DecorationTargetProps]: P extends keyof InjectedProps
    ? InjectedProps[P] extends DecorationTargetProps[P]
    ? DecorationTargetProps[P]
    : InjectedProps[P]
    : DecorationTargetProps[P];
};

// @public (undocumented)
export type MergeProps<TStateProps, TDispatchProps, TOwnProps, TMergedProps> =
(stateProps: TStateProps, dispatchProps: TDispatchProps, ownProps: TOwnProps) => TMergedProps;

// @public (undocumented)
type Omit_2<T, K extends keyof T> = Pick<T, Exclude<keyof T, K>>;
export { Omit_2 as Omit }

// @public (undocumented)
export interface Options<State = DefaultRootState, TStateProps = {}, TOwnProps = {}, TMergedProps = {}> extends ConnectOptions {
    areMergedPropsEqual?: (nextMergedProps: TMergedProps, prevMergedProps: TMergedProps) => boolean;

    areOwnPropsEqual?: (nextOwnProps: TOwnProps, prevOwnProps: TOwnProps) => boolean;

    areStatePropsEqual?: (nextStateProps: TStateProps, prevStateProps: TStateProps) => boolean;

    areStatesEqual?: (nextState: State, prevState: State) => boolean;

    forwardRef?: boolean;

    pure?: boolean;
}

// @public
export class Provider<A extends Action = AnyAction> extends Component<ProviderProps<A>> { }

// @public (undocumented)
export interface ProviderProps<A extends Action = AnyAction> {
    context?: Context<ReactReduxContextValue>;
    store: Store<any, A>;
}

// @public
export const ReactReduxContext: Context<ReactReduxContextValue>;

// @public (undocumented)
export interface ReactReduxContextValue<SS = any, A extends Action = AnyAction> {
    // (undocumented)
    store: Store<SS, A>;
    // (undocumented)
    storeState: SS;
}

// @public (undocumented)
export type ResolveArrayThunks<TDispatchProps extends ReadonlyArray<any>> =
TDispatchProps extends [infer A1, infer A2, infer A3, infer A4, infer A5, infer A6, infer A7, infer A8, infer A9]
? [HandleThunkActionCreator<A1>, HandleThunkActionCreator<A2>, HandleThunkActionCreator<A3>, HandleThunkActionCreator<A4>,
HandleThunkActionCreator<A5>, HandleThunkActionCreator<A6>, HandleThunkActionCreator<A7>, HandleThunkActionCreator<A8>, HandleThunkActionCreator<A9>]
: TDispatchProps extends [infer A1, infer A2, infer A3, infer A4, infer A5, infer A6, infer A7, infer A8]
? [HandleThunkActionCreator<A1>, HandleThunkActionCreator<A2>, HandleThunkActionCreator<A3>, HandleThunkActionCreator<A4>,
HandleThunkActionCreator<A5>, HandleThunkActionCreator<A6>, HandleThunkActionCreator<A7>, HandleThunkActionCreator<A8>]
: TDispatchProps extends [infer A1, infer A2, infer A3, infer A4, infer A5, infer A6, infer A7]
? [HandleThunkActionCreator<A1>, HandleThunkActionCreator<A2>, HandleThunkActionCreator<A3>, HandleThunkActionCreator<A4>,
HandleThunkActionCreator<A5>, HandleThunkActionCreator<A6>, HandleThunkActionCreator<A7>]
: TDispatchProps extends [infer A1, infer A2, infer A3, infer A4, infer A5, infer A6]
? [HandleThunkActionCreator<A1>, HandleThunkActionCreator<A2>, HandleThunkActionCreator<A3>, HandleThunkActionCreator<A4>, HandleThunkActionCreator<A5>, HandleThunkActionCreator<A6>]
: TDispatchProps extends [infer A1, infer A2, infer A3, infer A4, infer A5]
? [HandleThunkActionCreator<A1>, HandleThunkActionCreator<A2>, HandleThunkActionCreator<A3>, HandleThunkActionCreator<A4>, HandleThunkActionCreator<A5>]
: TDispatchProps extends [infer A1, infer A2, infer A3, infer A4] ? [HandleThunkActionCreator<A1>, HandleThunkActionCreator<A2>, HandleThunkActionCreator<A3>, HandleThunkActionCreator<A4>]
: TDispatchProps extends [infer A1, infer A2, infer A3] ? [HandleThunkActionCreator<A1>, HandleThunkActionCreator<A2>, HandleThunkActionCreator<A3>]
: TDispatchProps extends [infer A1, infer A2] ? [HandleThunkActionCreator<A1>, HandleThunkActionCreator<A2>]
: TDispatchProps extends [infer A1] ? [HandleThunkActionCreator<A1>]
: TDispatchProps extends Array<infer A> ? Array<HandleThunkActionCreator<A>>
: TDispatchProps extends ReadonlyArray<infer A> ? ReadonlyArray<HandleThunkActionCreator<A>>
: never
;

// @public (undocumented)
export type ResolveThunks<TDispatchProps> =
TDispatchProps extends { [key: string]: any }
? {
    [C in keyof TDispatchProps]: HandleThunkActionCreator<TDispatchProps[C]>
}
: TDispatchProps;

// @public (undocumented)
export type RootStateOrAny = AnyIfEmpty<DefaultRootState>;

// @public (undocumented)
export type Selector<S, TProps, TOwnProps = null> = TOwnProps extends null | undefined
? (state: S) => TProps
: (state: S, ownProps: TOwnProps) => TProps;

// @public
export type SelectorFactory<S, TProps, TOwnProps, TFactoryOptions> =
(dispatch: Dispatch<Action>, factoryOptions: TFactoryOptions) => Selector<S, TProps, TOwnProps>;

// @public
export function shallowEqual<T>(left: T, right: any): boolean;

// @public
export type Shared<
InjectedProps,
DecorationTargetProps
> = {
    [P in Extract<keyof InjectedProps, keyof DecorationTargetProps>]?: InjectedProps[P] extends DecorationTargetProps[P] ? DecorationTargetProps[P] : never;
};

// @public
export interface TypedUseSelectorHook<TState> {
    // (undocumented)
    <TSelected>(
    selector: (state: TState) => TSelected,
    equalityFn?: (left: TSelected, right: TSelected) => boolean
    ): TSelected;
}

// @public
export function useDispatch<TDispatch = Dispatch<any>>(): TDispatch;

// @public (undocumented)
export function useDispatch<A extends Action = AnyAction>(): Dispatch<A>;

// @public
export function useSelector<TState = DefaultRootState, TSelected = unknown>(
selector: (state: TState) => TSelected,
equalityFn?: (left: TSelected, right: TSelected) => boolean
): TSelected;

// @public
export function useStore<S = RootStateOrAny, A extends Action = AnyAction>(): Store<S, A>;

// (No @packageDocumentation comment for this package)

```