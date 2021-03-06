## API Report File for "@vue-composition-ui/pagination"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts

import type { Ref } from 'vue';
import type { ToRefs } from 'vue';

// @public (undocumented)
export function calcTotalPageSize(perPageSize: number, totalSize: number): number;

// @public (undocumented)
export function createRange(last: number, first?: number): number[];

// @public (undocumented)
export function isValidPageSize(currentPage: Ref<number>, totalPage: Ref<number>): boolean;

// @public
export function useGuaranteePageSize(currentPage: Ref<number>, totalPage: Ref<number>): void;

// @public (undocumented)
export function usePagination({ currentPage, perPageSize, totalSize, }: UsePaginationParams): ToRefs<UsePaginationReturnType>;

// @public (undocumented)
export interface UsePaginationParams {
    currentPage: Ref<number>;
    perPageSize: Ref<number>;
    totalSize: Ref<number>;
}

// @public (undocumented)
export interface UsePaginationReturnType {
    readonly currentEndSize: number;
    currentPage: number;
    readonly currentSize: number;
    readonly currentStartSize: number;
    readonly firstPage: number;
    readonly hasNextPage: boolean;
    readonly hasPrevPage: boolean;
    readonly isFirstPage: boolean;
    readonly isLastPage: boolean;
    readonly lastPage: number;
    readonly nextPage: number;
    readonly pageRange: number[];
    perPageSize: number;
    readonly prevPage: number;
    readonly totalPage: number;
    totalSize: number;
}

// @public (undocumented)
export function validatePageNumber(name: string, number: unknown): void;


// (No @packageDocumentation comment for this package)

```
